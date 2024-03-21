# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

**Logic Diagram**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: Moonesh P
RegisterNumber: 212223230126

```
module combinationalcircuit(A,B,C,D,F1);
input A,B,C,D;
output F1;
wire x1,x2,x3,x4,x5;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);
assign F1=x1|x2|x3|x4|x5;
endmodule
```
*/

**RTL realization**

![image](https://github.com/Moonesh0805/BOOLEAN_FUNCTION_MINIMIZATION/assets/138849189/d8eb8133-5598-409b-bad7-9722c959feb6)

**Output:**

**Timing Diagram**

![image](https://github.com/Moonesh0805/BOOLEAN_FUNCTION_MINIMIZATION/assets/138849189/85be9e80-1bd1-4f57-b5c4-b012803454c2)

**Truth Table**

![image](https://github.com/Moonesh0805/BOOLEAN_FUNCTION_MINIMIZATION/assets/138849189/c9c0b6e8-322f-4b91-a076-d0f960dec6b5)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

