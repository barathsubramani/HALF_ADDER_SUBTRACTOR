# HALF_ADDER_SUBTRACTOR

Implementation-of-Half-Adder-and-Half Subtractor-circuit

## AIM:

To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.

## Equipments Required:

Hardware – PCs, Cyclone II , USB flasher 

Software – Quartus prime Theory Adders are digital circuits that carry out the addition of numbers.

## Half Adder:

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/bd4a0b2c-cdbc-4184-ab08-81578f121e1f)

## Half Subtractor:

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

 ![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/d76b099c-513f-4e7c-843a-e2fd028a531a)

## Truthtable:
##Half adder

![image](https://github.com/barathsubramani/HALF_ADDER_SUBTRACTOR/assets/118542617/c1f57551-27c7-4ec5-90a5-2345ed6bfb92)


##Half subtractor

![image](https://github.com/barathsubramani/HALF_ADDER_SUBTRACTOR/assets/118542617/ff9834c7-24fe-4879-bacd-87fb6f0af70a)


## Procedure:

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


## Program:

Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

Developed by: Barath S

RegisterNumber: 212222230018

##Half adder
```
module half_adder(a,b,sum,carry);
input a,b;
output sum,carry; 
assign sum = a^b;
assign carry = a & b;
endmodule
```
##Half subtractor
```
module halfsub_top(a,b,D,Bo);
input a,b;
output D,Bo; // Outputs sum and carry for half adder:Outputs difference D,Borrow Bo for half subtractor
assign D = a ^ b;
  assign Bo = ~a & b;
endmodule
```
## RTL Schematic:
![image](https://github.com/barathsubramani/HALF_ADDER_SUBTRACTOR/assets/118542617/2b886f7b-00d4-47da-a685-6c153acad264)

## Output/TIMING Waveform:

##Half adder
![image](https://github.com/barathsubramani/HALF_ADDER_SUBTRACTOR/assets/118542617/3c19ab79-987e-4d83-a9f5-79bac2344350)



##Half subtractor
![image](https://github.com/barathsubramani/HALF_ADDER_SUBTRACTOR/assets/118542617/c4d34bc1-d02e-4bf1-b417-acdcb617876c)


## Result:
Thus implementation of Half Adder and Half subtractor circuit is running successfully.
