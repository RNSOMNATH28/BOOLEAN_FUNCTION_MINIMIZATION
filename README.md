# BOOLEAN_FUNCTION_MINIMIZATION
## Developed by: R N Somnath
## RegisterNumber:212224240158

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
module logic_function(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule

module logic_function(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule	

```
**RTL realization**
![image](https://github.com/user-attachments/assets/7fe01814-6c6e-4440-9cf6-c133f16a8246)
![image](https://github.com/user-attachments/assets/92e7009b-c775-4959-be94-fd06279c0bdd)


**Output:**
![image](https://github.com/user-attachments/assets/6d64f3d1-db2a-4641-9d9e-87b0c275ca0c)
![image](https://github.com/user-attachments/assets/b60fdafc-46ab-48e8-852d-5d538e0603a2)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

