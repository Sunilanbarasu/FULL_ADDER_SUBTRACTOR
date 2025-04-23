# FULL_ADDER_SUBTRACTOR

Reg No:212224220113

Date:19.03.2025

Implementation-of-Full-Adder-and-Full-subtractor-circuit

**AIM:**

To design a Full Adder and Full Subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime

**Full Adder and Full Subtractor**

**Full Adder**

Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin 

Carry = AB + ACin + BCin

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/0f30ba51-5ffb-4198-845f-18e054f675e7)

**Figure -1 FULL ADDER**

**Full Subtractor**

A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow.

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/02b24f51-ab51-4304-9ad6-7b81ffc1ead5)

Diff = A ⊕ B ⊕ Bin 

Borrow out = A'Bin + A'B + BBin

**Truthtable**

**Procedure**

Write the detailed procedure here

**Program:**
```
🔹 Full Adder Procedure
Inputs: A, B, Cin
Outputs: Sum, Cout

Sum = A ⊕ B ⊕ Cin

Cout = (A · B) + (B · Cin) + (Cin · A)

🔹 Full Subtractor Procedure
Inputs: A, B, Bin (borrow-in)
Outputs: Diff, Bout

Diff = A ⊕ B ⊕ Bin

Bout = (¬A · B) + (¬(A ⊕ B) · Bin)

```

**RTL Schematic**

![exp4(1)](https://github.com/user-attachments/assets/c2d0bd48-551d-414e-979e-ed906ba8d219)

![4(2)](https://github.com/user-attachments/assets/02b90689-ac44-4f9f-b832-03df2613a69e)



**Output Timing Waveform**
![exp4(1](https://github.com/user-attachments/assets/e459c270-e690-4996-affd-01a3f14ddd48)

![4(2](https://github.com/user-attachments/assets/b48009a7-e8af-46c2-93ac-aad64b2e48dc)


**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



