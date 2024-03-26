## vlsi-project
Project: Register File + ALU

![](https://progress-bar.dev/30/?title=Magic:&width=150)  ![](https://progress-bar.dev/100/?title=Logisim:&width=150)

**Milestone Checklist**
- [x] Preliminary project cell layouts: defines full schematic hierarchy and functionality.
- [ ] updated version of your milestone #2 writeup with any changes based on comments made. [ updated MS#2 submission with errors fixed (Canvas)]
  - [ ] conclusion is missing.
  - [x] drop multiplication for ALU
  - [x] schematic is not working
  - [x] demonstrate loading of values to the reg file and operating on them
  - [x] Please only include one test harness. It should consist of input pins, output ins, and a single part. 
  - [x] Please turn off the three-state inputs on your input pins
  - [x] DFFs have serious design flaws. Please fix Logisim simulation is not working.
  - [x] Many of the layouts submitted have design errors in them.
  - [x] Please include .cmd files to demonstrate that the layouts simulate proerly
- [x] complete Logisim/LogicWorks schematic (Canvas command)
- [x] .cmd test files for IRSIM (turnin command)
- [ ] partially complete set of Magic layouts for standard cells (these should only be submitted if DRC correct) (turnin command)
---
**Magic Hierarchy Development [Layer0 - Layer4]**

</br>
 -- ** *Layer0: transistor-level* **

  - [x] magic: OR2 gate
  - [x] magic: NOR2 gate
  - [x] magic: INV
  - [x] magic: OR3 gate
  - [x] magic: OR4 gate
  - [x] magic: NAND2 gate
  - [x] magic: XOR2 gate
  - [x] magic: AND2 gate
  - [x] magic: AND3 gate

</br> -- ** *Layer1: gate-level* **

  - [ ] magic: 1-bit MUX3
  - [ ] magic: 1-bit MUX2
  - [ ] magic: 1-bit MUX8
  - [ ] magic: 1-bit 3-to-8 Decoder
  - [ ] magic: 1-bit D Flip Flop
  - [x] magic: 1-bit full-Adder
  - [ ] magic: 1-bit full-Subtractor
  - [x] magic: 1-bit half-Adder
  - [x] magic: 1-bit half-Subtractor
  - [ ] magic: 4-bit AND2
  - [ ] magic: 4-bit OR2
  - [ ] magic: 4-bit NAND2
  - [ ] magic: 4-bit NOR2

</br> -- ** *Layer2: parts-level* **

  - [ ] magic: 4-bit MUX3
  - [ ] magic: 4-bit MUX8
  - [ ] magic: 4-bit Register
  - [ ] magic: 1-bit DFF with Enabler [merge MUX2 + DFF]
  - [ ] magic: 4-bit Adder
  - [ ] magic: 4-bit Subtractor

</br> -- ** *Layer3: block-level* **

  - [ ] magic: 4-bit Register File
  - [ ] magic: 4-bit ALU

</br> -- ** *Layer4: top-level [single block]* **

  - [ ] magic: 4-bit single-block [merge MUX3 + Register File + ALU]
</br>

---
</br>

**Progress**
- [x] Logisim functional (unless bugs/issues encountered)
- [x] magic gate layouts
- [x] make a single block as top level
- [x] make sure all magic simulates properly (will help us in the long run before we build the parts)
- [ ] build MUX3 in magic?
- [ ] build Register File in magic?
- [ ] build ALU in magic?

**Issues**
- [x] Fix DFF incorrect output
- [x] Fix Oscillation Apparent

**Workload**
- [x] Remove Multiplier
- [x] 8 bits to 4 bits
- [ ] Remove MUX3?
- [ ] cut down number of registers? (8 registers currently)

Abstract:
This project shows three crucial blocks: MUX3, Register File, and Arithmetic Logic Unit (ALU). The MUX3 selects data for storage in the Register File, which features 8 registers and dynamic address selection. The ALU performs arithmetic operations based on user selection, producing 4-bit results. Also, the ALU's output loops back to the MUX3, forming a crucial feedback loop for iterative calculations. Understanding these blocks is essential for understanding computing systems.

Parts: MUX3, Reg File, ALU

**Top level**

![Top](https://github.com/mrsamsonn/vlsi-project/assets/98930957/424d23e8-9215-4015-9972-f29a376ac115)


<img width="870" alt="Screenshot 2024-03-19 at 3 37 23 PM" src="https://github.com/mrsamsonn/vlsi-project/assets/98930957/2724f08f-e18e-4366-a934-91c9c3273caf">


</br>
</br>

# MUX3 Hierarchy

---

</br>

4 bit MUX3

![image](https://github.com/mrsamsonn/vlsi-project/assets/98930957/5a853507-5ef3-4111-9857-65be3b77bb49)


1 bit MUX

![3to1 Mux](https://github.com/mrsamsonn/vlsi-project/assets/98930957/3477f3a8-f016-4f9d-b6b5-b50f7bd1b1ff)

</br>
</br>

# Register File Hierarchy

---

</br>

Register File

<img width="862" alt="image" src="https://github.com/mrsamsonn/vlsi-project/assets/98930957/7beeacc0-43db-49b1-9af0-bd99ea1ce79e">


MUX8 (to cover 8 registers)

![image](https://github.com/mrsamsonn/vlsi-project/assets/98930957/3a117b66-c332-4932-b393-d25d4bb669b0)



4 bit Register

![image](https://github.com/mrsamsonn/vlsi-project/assets/98930957/bdcaee91-cc86-4134-aaae-b37431f57798)


D Flip Flop + MUX2[as enabler]

<img width="670" alt="image" src="https://github.com/mrsamsonn/vlsi-project/assets/98930957/600beece-724b-4916-a03c-d6780ff568af">

D Flip Flop

<img width="1124" alt="image" src="https://github.com/mrsamsonn/vlsi-project/assets/98930957/972b4de3-60a2-4bb7-8ef3-ef21c3290e14">


</br>
</br>

# ALU Hierarchy

---

</br>

ALU (Need one more logic to replace multiplier)

![ALU](https://github.com/mrsamsonn/vlsi-project/assets/98930957/8485986d-7a23-47a6-afa8-3933ee1e8197)

