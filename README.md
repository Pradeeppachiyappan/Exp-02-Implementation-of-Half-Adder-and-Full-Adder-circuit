# Exp-03-Implementation-of-Half-Adder-and-Full-Adder-circuit
## DATE :
## AIM :
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

## Equipments Required :
Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime

## Theory :
Adders are digital circuits that carry out addition of numbers.

#### Half Adder 
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

#### Full Adder 
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

 ![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)

#### Figure -01 HALF ADDER 


![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)

#### Figure -02 FULL ADDER 

### Procedure :

Connect the supply (+5V) to the circuit .

Switch ON the main switch .

If the output is 1, then the led glows.

## Program :
```
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: 212222240073
RegisterNumber: Pradeep Raj P

HALF ADDER

module exp_3(a,b,s,c);
input a,b;
output s,c;
assign s= a^b;
assign c = a&b;
endmodule

FULL ADDER

module exp_31(A,B,C,sum,carry);
input A,B,C;
output sum,carry;
assign sum= A^B^C;
assign carry = (A&B)|((A^B)&C);
endmodule
```
## RTL Diagram :
#### Half Adder
![image](https://github.com/Pradeeppachiyappan/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118707347/71392e76-ef48-433d-a53d-5bbaa02f3780)

#### Full Adder 
![image](https://github.com/Pradeeppachiyappan/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118707347/c1ecddfc-9148-48ce-86b8-2d9cd0df1ba9)

### TRUTH TABLE :
#### Half Adder
![image](https://github.com/Pradeeppachiyappan/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118707347/a60c73ca-eff2-4077-ae64-d7e50e8899bd)

#### Full Adder
![image](https://github.com/Pradeeppachiyappan/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118707347/9dd2ec1e-b860-48f0-9798-0718e233dd2e)


### Output Waveform :
#### Half Adder
![image](https://github.com/Pradeeppachiyappan/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118707347/29652277-0103-49e3-afa4-ea82e32033c1)

#### Full Adder
![image](https://github.com/Pradeeppachiyappan/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118707347/d95bb22d-cd8b-4337-ab07-62d328f58e49)
 
### Result:
Thus the implementation of half adder and full adder circiut are stuided and the truth table for different logic gates .


