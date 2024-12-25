## NAME: A.PRAVEENA
## REG NO: 24006885
## EXPERIMENT 4: FULL_ADDER_SUBTRACTOR

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
(i) FULL ADDER
![Screenshot 2024-12-25 141610](https://github.com/user-attachments/assets/c7fc8c08-b8ba-408a-98f1-aa321850d3a9)
(ii) FULL SUBTRACTOR
![Screenshot 2024-12-25 141622](https://github.com/user-attachments/assets/3ef357a6-3ebb-4a45-864e-ce9f0cfb096f)

**Procedure**
1.Type the program in Quartus software.

2.Compile and run the program.

3.Generate the RTL schematic and save the logic diagram.

4.Create nodes for inputs and outputs to generate the timing diagram.

5.For different input combinations generate the timing diagram.

**Program:**
i)FULL ADDER

module fa(a,b,cin,sum,carry);
input a,b,cin;
output sum,carry;
assign sum=( (a ^ b)^cin);
assign carry= ( (a & b)| ( cin &(a ^ b )));
endmodule

ii)FULL SUBTRACTOR

module fs(a,b,bin,difference,borrow);
input a,b,bin;
output difference,borrow;
assign difference= ( (a ^ b)^bin);
assign borrow= ( ( ~a & b)| ( bin & (~(a ^ b ))));
endmodule

**RTL Schematic**
FULL ADDER
![Screenshot 2024-12-25 142133](https://github.com/user-attachments/assets/066486a9-7dae-421d-bce2-3a8f2a80d1f5)

FULL SUBTRACTOR
![image](https://github.com/user-attachments/assets/f17def78-23ff-4412-bbf2-c9c1973b49a9)


**Output Timing Waveform**
FULL ADDER
![image](https://github.com/user-attachments/assets/76107640-a99a-4abe-a81c-34913c3a2d01)

FULL SUBTRACTOR
![Screenshot 2024-12-25 142428](https://github.com/user-attachments/assets/66c8d0dc-8635-4349-bd9f-eba435614b5f)


**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



