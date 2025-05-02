# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

Boolean Algebra is a branch of algebra that deals with boolean values—true and false. It is fundamental to digital logic design and computer science, providing a mathematical framework for describing logical operations and expressions.

**Logic Diagram**

![Screenshot 2025-04-21 180356](https://github.com/user-attachments/assets/b988b6dc-cf41-499e-9cf6-e3954b4865c9)

F1:
![Screenshot 2025-04-21 180410](https://github.com/user-attachments/assets/1f4405aa-1ea9-47d6-9467-246e5ef3fa04)

F2:
![Screenshot 2025-04-21 180419](https://github.com/user-attachments/assets/27f6dd98-ef85-4b9d-8d1e-04cf42342d9b)

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: VENKATA MOHAN N RegisterNumber: 212224230298*/

F1:
```
module funct1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule
```

F2:
```
module funct2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule
```

**RTL**

F1:
![Screenshot 2025-04-21 180445](https://github.com/user-attachments/assets/3d70639f-c554-49db-b2b1-b7c6d8d190a9)

F2:
![Screenshot 2025-04-21 180456](https://github.com/user-attachments/assets/a6935cca-ced0-4220-ada7-4a150ced6839)

**Timing Diagram**

F1:
![Screenshot 2025-04-21 180509](https://github.com/user-attachments/assets/a46e269e-ccbc-4d9d-b0be-f95c01ed6c24)

F2:
![Screenshot 2025-04-21 180522](https://github.com/user-attachments/assets/32f7e3b9-9ab7-4f74-98c2-9bf931dbd311)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.


