![image](https://github.com/user-attachments/assets/c78b026c-bcf0-4ce5-848b-b04dbd3531d8)# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

**Logic Diagram**
FUNCTION 1 K-MAP

![Screenshot 2024-12-11 140401](https://github.com/user-attachments/assets/4911dc87-09e3-4a7c-a851-66027cac30c6)

FUNCTION 2K-MAP
  
![Screenshot 2024-12-11 140531](https://github.com/user-attachments/assets/4d2ba29d-eed9-4c70-b49b-e798a2a49b09)

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
FUNCTION 1
module funct1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule
FUNCTION 2
module funct2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule

FUNCTION 1
![Screenshot 2024-12-11 140754](https://github.com/user-attachments/assets/5e010837-625d-43a3-9d13-76c4cc0cb8d7)
FUNCTION 2

![Screenshot 2024-12-11 141014](https://github.com/user-attachments/assets/393550c9-78ee-4ca9-91d2-830aac7c6d89)


/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:S.YOGESH
RegisterNumber:24001573 */


**RTL realization**

**Output:**

**RTL**
FUNCTION 1
![Screenshot 2024-12-11 141129](https://github.com/user-attachments/assets/681ddd5a-2cf5-4650-af6f-14bb7d8088d3)

FUNCTION 2
![Screenshot 2024-12-11 141138](https://github.com/user-attachments/assets/3d52669a-295a-49e8-94d5-23a22ba87c96)

**Timing Diagram**
FUNCTION 1
![Screenshot 2024-12-11 141226](https://github.com/user-attachments/assets/1502827a-19e1-4be5-b381-4dce37869f52)

FUNCTION 2

![Screenshot 2024-12-11 141237](https://github.com/user-attachments/assets/64b00edb-298f-444a-9eeb-fd0dd5d89dc1)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

