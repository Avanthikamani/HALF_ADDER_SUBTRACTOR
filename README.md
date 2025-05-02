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



**Half Subtractor**

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

 ![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/d76b099c-513f-4e7c-843a-e2fd028a531a)


**Truthtable**
![Screenshot 2025-05-02 132505](https://github.com/user-attachments/assets/ed8c7e8e-8159-488b-a756-a60ceb13d144)
![Screenshot 2025-05-02 132516](https://github.com/user-attachments/assets/3ac5c25b-0325-47b7-a3f5-0cb84eb50501)

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:
module exp3(a,b,sum,carry);
input a,b;
output sum,carry;
assign sum= (a ^ b);
assign carry= ( a & b);
endmodule
module exp3(a,b,difference,borrow);
input a,b;
output difference,borrow;
assign difference= (a ^ b);
assign borrow= ( ~a & b);
endmodule

Developed by:Avanthika M RegisterNumber:212224110009*/

**RTL Schematic**
![Screenshot 2025-05-01 182831](https://github.com/user-attachments/assets/2c80d374-51d4-493d-85f0-5add09e84039)
![Screenshot 2025-05-01 184942](https://github.com/user-attachments/assets/5795cec1-3b87-45aa-b223-106e0dad28fc)

**Output/TIMING Waveform**
![Screenshot 2025-05-01 182950](https://github.com/user-attachments/assets/b8323055-453f-468b-ab15-5e84705c1e60)
![Screenshot 2025-05-01 185624](https://github.com/user-attachments/assets/37aeda3f-51ed-4fd5-a0b7-2e1449baa1b2)


**Result:**
Thus, the half adder and half subtractor verilog program has been sucessfully executed
