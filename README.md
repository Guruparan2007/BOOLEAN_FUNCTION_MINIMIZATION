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

**BOOLEAN MINIMIZATION**


![Screenshot 2024-12-23 131636](https://github.com/user-attachments/assets/5f78b1b1-72e9-407a-8a40-4a0f58cb2872)


![Screenshot 2024-12-23 131655](https://github.com/user-attachments/assets/2e6670ed-68f5-47c9-9a6d-67e086e63f2f)


**TRUTHTABLE**

F1
 ![Screenshot 2024-12-23 131740](https://github.com/user-attachments/assets/3363f583-0ed6-4476-b955-eb8ee7d9b760)

F2
![Screenshot 2024-12-23 131757](https://github.com/user-attachments/assets/48137267-9196-4073-8921-8335e8049323)

**Program:**

~~~
 i)
 module funct1(a,b,c,d,f1);
 input a,b,c,d;
 output f1;
 assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
 endmodule
 ii)
 module funct2(w,x,y,z,f2);
 input w,x,y,z;
 output f2;
 assign f2=((~y & z)|( w & y )|(x & y));
 endmodul
~~~

Developed by: GURUPARAN GRegisterNumber: 24001677

**RTL**

![Screenshot 2024-12-23 131827](https://github.com/user-attachments/assets/34e92ec3-19f4-4d7b-8c6b-0eff94f36488)


![Screenshot 2024-12-23 131843](https://github.com/user-attachments/assets/7bda43dc-5f9f-41ff-811e-df61b1d50ae5)



**Timing Diagram**


![Screenshot 2024-12-23 131900](https://github.com/user-attachments/assets/d19b6c9b-aaa9-44bf-a86d-51e491ab7f4c)


![Screenshot 2024-12-23 131918](https://github.com/user-attachments/assets/422d29bd-4049-42ef-83a5-fe2df8109893)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

