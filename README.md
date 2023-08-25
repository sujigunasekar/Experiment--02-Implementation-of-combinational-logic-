# Experiment--02-Implementation-of-combinational-logic

 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D

 
 
 
## Equipments Required:
   Hardware – PCs, Cyclone II , USB flasher
   Software – Quartus prime


## Theory
Logic gates are electronic circuits which perform logical functions on one or more inputs to produce one output.

Logic gates are electronic circuits which perform logical functions on one or more inputs to produce one output. F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

1.AND gate The AND gate is an electronic circuit that gives a high output (1) only if all its inputs are high. A dot (.) is used to show the AND operation i.e. A.B or can be written as AB Y= A.B

2.OR gate The OR gate is an electronic circuit that gives a high output (1) if one or more of its inputs are high. A plus (+) is used to show the OR operation. Y= A+B
 

## Logic Diagram

## Procedure
1.Create a project with required entities.

2.Create a module along with respective file name.

3.Run the respective programs for the given boolean equations.

4.Run the module and get the respective RTL outputs.

5.Create university program(VWF) for getting timing diagram.

6.Give the respective inputs for timing diagram and obtain the results.
## Program:
```
Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
Developed by: Suji.G
RegisterNumber:  212222230152
module f1(A,B,C,D,F1);
input A,B,C,D;
output F1;
wire p,q,r,s,t;
assign p = (~A & ~B & ~C & ~D);
assign q = (A & ~C & ~D);
assign r = (~B & C & ~D);
assign s = (~A & B & C & D);
assign t = (B & ~C & D);
assign F1 = p | q | r | s | t;
endmodule
````
## RTL realization
![Screenshot 2023-08-25 100858](https://github.com/sujigunasekar/Experiment--02-Implementation-of-combinational-logic-/assets/119559822/39d8e82b-1986-4090-895a-5264ae96a9c3)

## Output:
![Screenshot 2023-08-25 093524](https://github.com/sujigunasekar/Experiment--02-Implementation-of-combinational-logic-/assets/119559822/51fcb51e-45cc-4011-90fb-d378af321103)

## Truth Table:
![Screenshot 2023-08-25 094923](https://github.com/sujigunasekar/Experiment--02-Implementation-of-combinational-logic-/assets/119559822/ba6148df-1755-413c-94d9-cf5c79c43a73)





## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
