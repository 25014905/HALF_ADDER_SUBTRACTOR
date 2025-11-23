# HALF_ADDER_SUBTRACTOR

Implementation-of-Half-Adder-and-Half Subtractor-circuit

**AIM:**

To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher 

Software – Quartus prime Theory Adders are digital circuits that carry out the addition of numbers.

**Half Adder**

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits...

Sum = A’B+AB’ =A ⊕ B Carry = AB

![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/bd4a0b2c-cdbc-4184-ab08-81578f121e1f)

Figure -01 HALF ADDER

**Half Subtractor**

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

 ![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/d76b099c-513f-4e7c-843a-e2fd028a531a)

Figure -02 HALF Subtractor

**Truthtable**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

 Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

Developed by: Mirdula D   RegisterNumber:25014905

***Half-adder***

module expadd(a,b,sum,carry);

input a,b;

output sum, carry;

xor g1(sum, a,b);

assign carry =a&b;

endmodule

***Half-subtractor***

module exp3 (a,b, diff, borrow);

input a,b;

output diff, borrow;

xor g1(diff, a,b);

assign borrow =~a&b;

endmodule

**RTL Schematic**


<img width="1772" height="942" alt="image" src="https://github.com/user-attachments/assets/39eb8848-d652-49b3-99b1-8c4176f7cefe" />


<img width="1919" height="1021" alt="image" src="https://github.com/user-attachments/assets/1abfd23a-8e60-46d5-98f8-5b634f91ba9a" />

**Output/TIMING Waveform**


<img width="1910" height="993" alt="image" src="https://github.com/user-attachments/assets/61a6183c-8acf-4f6c-aa47-8ea56bf73e22" />


<img width="1912" height="1011" alt="image" src="https://github.com/user-attachments/assets/fd5fffaa-19cf-482a-8dfd-2d29931356a0" />


**Result:**

Thus designed a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.
