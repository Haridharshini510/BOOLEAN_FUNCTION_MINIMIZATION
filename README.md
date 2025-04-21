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
F1

module exp3(A,B,C,D,F1);
input A,B,C,D;
output F1;
wire w1,w2,w3;
assign w1= (~B)&(~D);
assign w2= A&B&(~C);
assign w3= (~A)&B&D;
assign F1= w1|w2|w3;
endmodule

F2
module exp3a(w,x,y,z,F2);
input w,x,y,z;
output F2;
wire w1,w2,w3;
assign w1= w&y;
assign w2= (y)&(~z);
assign w3= x&y;
assign F2= w1|w2|w3;
endmodule




**RTL realization**

![Screenshot (411)](https://github.com/user-attachments/assets/5b7ebdbb-69f8-40f9-bf48-48fbabf9e4d4)

![Screenshot (423)](https://github.com/user-attachments/assets/4249ad4a-40a5-4cad-9551-e1e29184e177)

**Timing Diagram**
![Screenshot (412)](https://github.com/user-attachments/assets/6a6791ed-71ad-47e9-9f13-957401e90541)

![Screenshot (422)](https://github.com/user-attachments/assets/fc972754-8e9c-4e48-bd22-dab88c46b1cd)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

