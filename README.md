Date:12.03.2025
# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**
To implement and verify a logic function in Quartus using Verilog, first define the logic expression in a Verilog module. Then, write a testbench to simulate all possible input combinations. Use the Quartus simulation tools (like ModelSim) to observe output responses and confirm correctness. Finally, validate the results using the truth table of the function.

**Logic Diagram**
![Screenshot 2025-04-15 111918](https://github.com/user-attachments/assets/2e43434e-9e2b-42a3-9d8f-79dd39b8ca6a)

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

```
Exp 2:
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

Developed by: RegisterNumber:212224220113
Name:Sunil.A


**RTL realization**

![de exp 2 (1)](https://github.com/user-attachments/assets/96c2cbf5-f24b-4298-8ffd-8306265f1d5c)


![de exp 2(2)](https://github.com/user-attachments/assets/3be2738b-39f5-4ae2-8387-c12e69c94ed9)



**Timing Diagram**
![de exp 2(1)](https://github.com/user-attachments/assets/f5d9ce83-e8ab-489b-95d2-7b4ff1470722)
![DE exp2(@2)](https://github.com/user-attachments/assets/dd8a9a80-df5a-4b53-8aa2-84f8e6b3ff67)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

