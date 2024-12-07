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
```
module funct1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule


module funct2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule
```
/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: RegisterNumber:*/


**RTL realization**

![Screenshot 2024-11-26 173934](https://github.com/user-attachments/assets/1f4d7f6b-9334-4438-8bec-f3fba5c7f756)

![Screenshot 2024-11-26 175703](https://github.com/user-attachments/assets/8e376d2b-d837-480f-b78c-0bc0802bbb43)


**Timing Diagram**

![Screenshot 2024-11-26 174232](https://github.com/user-attachments/assets/ffb5f7a4-dc01-4d06-aba9-9597898d5317)
![Screenshot 2024-11-26 180209](https://github.com/user-attachments/assets/f2c4173b-8b84-4e96-81d9-e34006458db1)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

