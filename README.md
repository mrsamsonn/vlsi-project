## vlsi-project
Project: Register File + ALU

**Progress**
- [x] Logisim functional (unless bugs/issues encountered)
- [x] magic gate layouts
- [ ] make a single block as top level
- [ ] make sure all magic simulates properly (will help us in the long run before we build the parts) 

**Issues**
- [x] Fix DFF incorrect output
- [x] Fix Oscillation Apparent

**Workload**
- [x] Remove Multiplier
- [x] 8 bits to 4 bits
- [ ] Remove MUX3?
- [ ] cut down number of registers? (8 registers currently)

Abstract:
This project shows three crucial blocks: MUX3, Register File, and Arithmetic Logic Unit (ALU). The MUX3 selects data for storage in the Register File, which features 8 registers and dynamic address selection. The ALU performs arithmetic operations based on user selection, producing 8-bit results. Also, the ALU's output loops back to the MUX3, forming a crucial feedback loop for iterative calculations. Understanding these blocks is essential for understanding computing systems.

Parts: MUX3, Reg File, ALU

**Top level**

![main](https://github.com/mrsamsonn/vlsi-project/assets/98930957/8597835f-14f4-42f0-9610-4db2c482ba72)

</br>
</br>

# MUX3 Hierarchy

---

</br>

8 bit MUX3

![8 bit 3to1MUX](https://github.com/mrsamsonn/vlsi-project/assets/98930957/a44f0049-fbc7-4851-b8b7-1f4f8feb97f4)

1 bit MUX

![3to1 Mux](https://github.com/mrsamsonn/vlsi-project/assets/98930957/3477f3a8-f016-4f9d-b6b5-b50f7bd1b1ff)

</br>
</br>

# Register File Hierarchy

---

</br>

Register File

![Reg File](https://github.com/mrsamsonn/vlsi-project/assets/98930957/d1bd9406-3cac-4b56-8874-4eb18b8319ac)

MUX8 (to cover 8 registers)

![8 bit MUX](https://github.com/mrsamsonn/vlsi-project/assets/98930957/634455a2-917d-4b63-84a9-a41fbe90f3fb)


8 bit Register

<img width="924" alt="image" src="https://github.com/mrsamsonn/vlsi-project/assets/98930957/9b0ddc9a-6b17-4d85-a415-f31b6a4f8126">

D Flip Flop + MUX2[as enabler]

<img width="670" alt="image" src="https://github.com/mrsamsonn/vlsi-project/assets/98930957/600beece-724b-4916-a03c-d6780ff568af">

D Flip Flop

<img width="1124" alt="image" src="https://github.com/mrsamsonn/vlsi-project/assets/98930957/972b4de3-60a2-4bb7-8ef3-ef21c3290e14">


</br>
</br>

# ALU Hierarchy

---

</br>

ALU

![ALU](https://github.com/mrsamsonn/vlsi-project/assets/98930957/a0bab6ac-c0d0-4a39-aeb7-3d22dff6c33f)
