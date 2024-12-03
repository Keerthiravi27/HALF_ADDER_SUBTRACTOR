# HALF_ADDER_SUBTRACTOR

Implementation-of-Half-Adder-and-Half Subtractor-circuit

**AIM:**

To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher 

Software – Quartus prime Theory Adders are digital circuits that carry out the addition of numbers.

**Half Adder**

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/bd4a0b2c-cdbc-4184-ab08-81578f121e1f)

Figure -01 HALF ADDER


**Half Subtractor**

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

 ![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/d76b099c-513f-4e7c-843a-e2fd028a531a)

Figure -02 HALF Subtractor


**Truthtable**!
![WhatsApp Image 2024-12-03 at 09 34 42_8a030e75](https://github.com/user-attachments/assets/2699ea4d-93ab-4cb6-b401-cbcdc1c79eae)
![WhatsApp Image 2024-12-03 at 09 34 55_61bd4f6c](https://github.com/user-attachments/assets/937f5baa-6c1e-411e-bc72-b81f30f46738)




**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
half subtractor
module halfsub2(a,b,difference,borrow);
input a,b;
output difference,borrow;
assign differnce=(a^b);
assign borrow=(~a&b);
endmodule
half adder
module halfadder2(a,b,sum,carry);
input a;
input b;
output sum,carry;
assign sum=a^b;
assign carry=a+b;
endmodule


/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

Developed by: RegisterNumber:*/24900170 Keerthana R

**RTL Schematic**
![WhatsApp Image 2024-12-03 at 09 31 21_32adde88](https://github.com/user-attachments/assets/5192a5f0-e4e7-4665-a3ba-72016680ce92)
![Screenshot (32)](https://github.com/user-attachments/assets/02aa2ea7-cc4f-4331-ade2-ce1f05e1ef30)




**Output**![Screenshot (34)](https://github.com/user-attachments/assets/c9d72aa8-aaf7-4891-80de-d451ea55c043)
![Screenshot (35)](https://github.com/user-attachments/assets/f3bca415-c1d2-4b53-b57a-10967d474b87)



**Result:**
Thus designed a half adder and half subtractor circuit and verified its truth table in Quartus usind verilog programming.
