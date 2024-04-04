# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**
Theory A combinational circuit is a circuit in which the output depends on the present combination of inputs. Combinational circuits are made up of logic gates. The output of each logic gate is determined by its logic function. Combinational circuits can be made using various logic gates, such as AND gates, OR gates, and NOT gates.   


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: Yuvan M

RegisterNumber:212223240188
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

**RTL realization**
![exp_22](https://github.com/Yuvan291205/BOOLEAN_FUNCTION_MINIMIZATION/assets/138849170/be307360-7eda-44f5-937b-7cdb50c75180)


**RTL**
![FAF](https://github.com/Yuvan291205/BOOLEAN_FUNCTION_MINIMIZATION/assets/138849170/18a918a3-5b3f-4e71-9b28-388a47004232)


**Timing Diagram**
![Screenshot 2024-03-10 174903](https://github.com/Yuvan291205/BOOLEAN_FUNCTION_MINIMIZATION/assets/138849170/b06b92fd-c8ae-4e4e-9674-785a57ce3f75)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

