# FULL_ADDER_SUBTRACTOR
Date:19.03.2025
Reg no 212224220113
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



**Program:**

Program: FULL ADDRER:
module faexp(a,b,cin,sum,carry);
input a,b,cin;
output sum,carry;
assign sum=( (a ^ b)^cin);
assign carry= ( (a & b)| ( cin &(a ^ b )));
endmodule
FULL SUBTRACTOR:
module fsexp(a,b,bin,difference,borrow);
input a,b,bin;
output difference,borrow;
assign difference= ( (a ^ b)^bin);
assign borrow= ( ( ~a & b)| ( bin & (~(a ^ b ))));
endmodule


**RTL Schematic**

![exp4(1)](https://github.com/user-attachments/assets/0b0b6d50-37ab-4aa6-b33f-21370b96e81c)

![4(2)](https://github.com/user-attachments/assets/0173c032-1b0a-4bce-907d-931ded354d56)


**Output Timing Waveform**
![exp4(1](https://github.com/user-attachments/assets/bc5f8c90-e60f-4016-a4d0-dd671862a9d1)

![4(2](https://github.com/user-attachments/assets/17aa1078-f966-4002-a584-6f89369a7e79)



**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



