# Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit

# Implementation-of-Half-Adder-and-Full-Adder-circuit
### AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

### Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime
Theory
Adders are digital circuits that carry out addition of numbers.

### Half Adder
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

### Full Adder
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

 ![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)

#### Figure -01 HALF ADDER 


![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)

#### Figure -02 FULL ADDER 

### Procedure

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.
### Program:
```
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: Kowsalya M
RegisterNumber:  212222230069
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: PRIYANKA.A
RegisterNumber: 212222230113
Half adder program:
module HalfAdder(A,B,sum,carry);
input A,B;
output sum,carry;
assign sum= A^B;
assign carry = A&B;
endmodule
Full adder program:
module FullAdder(A,B,Cin,sum,carry);
input A,B,Cin;
output sum,carry;
assign sum= A^B^Cin;
assign carry = (A&B)|((A^B)&Cin);
endmodule
```
## Output:
### RTL:
#### Half adder:
![R3 1](https://github.com/Kowsalyasathya/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118671457/916230e2-45bb-4223-bcb1-80161d7f0d88)
#### Full adder:
![R3 1](https://github.com/Kowsalyasathya/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118671457/dca294e0-565f-4d36-bca0-9e581fb9b642)
### TRUTH TABLE 
#### Half adder:
![R3 2](https://github.com/Kowsalyasathya/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118671457/8d3ce1a7-14fa-4358-83e6-98ede74d1e1a)

#### Full adder:
![R3 3](https://github.com/Kowsalyasathya/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118671457/cc258e95-42fe-4369-b7f3-b43bbb6aeadd)
### Waveform:
#### Half adder:
![R3 3](https://github.com/Kowsalyasathya/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118671457/449f24fe-1ffb-4132-93e0-6e45885c1e6e)

#### Full adder:
![R3 4](https://github.com/Kowsalyasathya/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118671457/64f957fd-0b6d-4832-a9b1-61726af57dfc)

### Result:
Thus the Implementation of Half Adder and Full Adder circuit are studied and the truth table for different logic gates are verified.
