# Experiment--02-Implementation-of-combinational-logic
Implementation of combinational logic gates
 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
F2=xy’z+x’y’z+w’xy+wx’y+wxy
 
 
 
## Equipments Required:
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime


## Theory
 

## Logic Diagram
## Procedure
## Program:
~~~~
module kmap(w,x,y,z,F1);
input w,x,y,z;
output F1;
wire wbar,xbar,ybar,zbar,a,b,c,d,e;
assign wbar=~w;
assign xbar=~x;
assign ybar=~y;
assign zbar=~z;
assign a=wbar&xbar&ybar&zbar;
assign b=wbar&x&zbar;
assign c=w&ybar&zbar;
assign d=wbar&xbar&y;
assign e=xbar&ybar&z;
assign F1=a|b|c|d|e;
endmodule
~~~~
## RTL realization
![kmap logic gate](https://github.com/Mario-Viofer-J/Experiment--02-Implementation-of-combinational-logic-/assets/144979232/5af60982-2450-4f68-9f38-771d013363c3)

## Output:
## Truth Table
![image](https://github.com/Mario-Viofer-J/Experiment--02-Implementation-of-combinational-logic-/assets/144979232/50b0e972-41f9-4b2f-9994-cd3aecd4da0c)

## Timing Diagram
![kmap waveform](https://github.com/Mario-Viofer-J/Experiment--02-Implementation-of-combinational-logic-/assets/144979232/483da37f-8482-4670-a944-99be9777bc3f)


## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
