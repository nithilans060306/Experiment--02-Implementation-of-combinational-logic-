## Name: Nithilan S

## RegisterNumber: 23013463

## ExperimentNumber: 02 
# Experiment -02 Implementation of combinational logic gates

## Aim:
To implement the given logic function verify its operation in Quartus using Verilog programming.
F1 = A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D


## Equipments Required:
```
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime
```

## Theory:
A combinational circuit is a circuit in which the output depends on the present combination of inputs. Combinational circuits are made up of logic gates. The output of each logic gate is determined by its logic function. Combinational circuits can be made using various logic gates, such as AND gates, OR gates, and NOT gates.

## Procedure:
```
Connect the supply (+5V) to the circuit Switch ON
the main switch Press the switches for inputs “A” and “B”.
The switch is ON state when 1 is pressed. The switch is OFF state when 0 is pressed.
If the output is 1, then the bulb glows. 
Check all the gates following the same procedure.
```

## Program:
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

## RTL realization:
![image](https://github.com/nithilans060306/Experiment--02-Implementation-of-combinational-logic-/assets/147473026/a1983d15-c493-4015-bbc3-2b640c420b50)

## Truth table:
![image](https://github.com/nithilans060306/Experiment--02-Implementation-of-combinational-logic-/assets/147473026/f2cfdd4d-ba36-460c-8c4e-edceb14e351c)

## Timing Diagram:
![image](https://github.com/nithilans060306/Experiment--02-Implementation-of-combinational-logic-/assets/147473026/7513f89d-013d-4493-9aa0-9befa49e7056)

## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
