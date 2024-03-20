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

![Reg File](https://github.com/mrsamsonn/vlsi-project/assets/98930957/d1bd9406-3cac-4b56-8874-4eb18b8319ac)

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

![image](https://github.com/mrsamsonn/vlsi-project/assets/98930957/9b3193b2-cb6f-4e3f-a029-e358ea8a41ae)
