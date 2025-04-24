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
Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: RegisterNumber: 212223040233

```
module Boolean_min(A,B,C,D,W,X,Y,Z,F1,F2);
input A,B,C,D,W,X,Y,Z;
wire x1,x2,x3,x4,x5,x6,x7,x8,x9,x10;
output F1,F2;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);
assign x6=(X)&(~Y)&(Z);
assign x7=(~X)&(~Y)&(Z);
assign x8=(~W)&(X)&(Y);
assign x9=(W)&(~X)&(Y);
assign x10=(W)&(X)&(Y);
assign F1=x1|x2|x3|x4|x5;
assign F2=x6|x7|x8|x9|x10;
endmodule

```
**RTL realization**

![image](https://github.com/user-attachments/assets/b2d6d2ee-227d-4573-bd83-6242fcee84e2)

![image](https://github.com/user-attachments/assets/a6472fbc-64d8-4ca2-8964-5b9100091cbd)

**RTL**
![image](https://github.com/user-attachments/assets/015c9195-d17e-4e1c-a7e2-0a5e481b0277)

![image](https://github.com/user-attachments/assets/1ac61ccd-9d19-46a7-8d35-d8645d479348)

**OUTPUT**
![image](https://github.com/user-attachments/assets/a3f64e40-a02d-4c3b-accb-cbf7714c548b)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

