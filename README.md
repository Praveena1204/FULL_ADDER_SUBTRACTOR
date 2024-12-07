## NAME: A.PRAVEENA
## REGISTER N0: 24006885
# EXPERIMENT NO:4  FULL_ADDER_SUBTRACTOR

Implementation-of-Full-Adder-and-Full-subtractor-circuit

## AIM:

To design a Full Adder and Full Subtractor circuit and verify its truth table in Quartus using Verilog programming.

## Equipments Required:

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime

## Full Adder and Full Subtractor

## Full Adder

Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin 

Carry = AB + ACin + BCin

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/0f30ba51-5ffb-4198-845f-18e054f675e7)

## Figure -1 FULL ADDER

## Full Subtractor

A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow.

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/02b24f51-ab51-4304-9ad6-7b81ffc1ead5)

Diff = A ⊕ B ⊕ Bin 

Borrow out = A'Bin + A'B + BBin

## Truthtable
![Screenshot 2024-12-06 205017](https://github.com/user-attachments/assets/dccd430c-8f1c-48ed-a95c-c03f85d8c513)
![Screenshot 2024-12-06 205002](https://github.com/user-attachments/assets/9c36d812-854a-469e-b4f3-66fb301a2aa5)


## Procedure

1.Open Quartus II and create a new project.

2.Use schematic design entry to draw the full adder circuit and full subractor circuit.

3.The circuit consists of XOR, AND, and OR gates.

4.Compile the design, verify its functionality through simulation. 

5.Implement the design on the target device and program it.

## Program:
![Screenshot 2024-12-06 204538](https://github.com/user-attachments/assets/fb177023-c267-4ceb-af61-7541259a5b5f)

## RTL Schematic
![Screenshot 2024-12-06 204525](https://github.com/user-attachments/assets/695885b4-b480-48fa-a6bb-ca1d32fac25c)

## Output Timing Waveform
![Screenshot 2024-12-06 210343](https://github.com/user-attachments/assets/8a1a372c-161e-49ba-bd83-4df3d41da1a9)
![Screenshot 2024-12-06 210328](https://github.com/user-attachments/assets/015fd41d-c33c-4722-838a-954228746750)


## Result:
Thus the Full Adder and Full Subtractor circuits are designed and the truth tables were verified using Quartus software.



