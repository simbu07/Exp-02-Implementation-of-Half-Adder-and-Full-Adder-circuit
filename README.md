# Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit

# Implementation-of-Half-Adder-and-Full-Adder-circuit
## AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

## Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime
## Theory
Adders are digital circuits that carry out addition of numbers.

### Half Adder
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

### Full Adder
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

 ![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)

### Figure -01 HALF ADDER 


![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)

#### Figure -02 FULL ADDER 

## Procedure

1.Connect the supply (+5V) to the circuit

2.Switch ON the main switch

3. If the output is 1, then the led glows.
### 
## Program:
```
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: Silambarsan K
RegisterNumber:  212221230101
```
### Half adder program:
```
module half_adder(a,b,sum,carry);
input a,b;
output sum,carry;
assign sum = (a^b);
assign carry = (a&b);
endmodule
``` 
### Full adder program:
```
module full_adder (a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum = (a^b^c);
assign carry = ((a&b)|(a^b)&c);
endmodule
```
### Output:
#### Logic symbol & Truthtable
Half adder:
![DIG2](https://user-images.githubusercontent.com/94154683/164457046-bfdb27f7-66f8-4a5f-b1a9-46e3b3c312c7.PNG)

Full adder:
![RTL realization](https://user-images.githubusercontent.com/94154683/164457085-f0929a1f-0001-4937-960d-1e386ca6c9bd.PNG)


### RTL
Half adder:
![DIG2](https://user-images.githubusercontent.com/94154683/164240824-a7b58108-4a64-413d-a691-86d2e2cf4b99.PNG)

Full adder:
![RTL realization](https://user-images.githubusercontent.com/94154683/164455620-be9d5c59-e310-411b-bfd9-60065080e8c7.PNG)

### TIMING DIAGRAM
Half adder:
![DIG2](https://user-images.githubusercontent.com/94154683/164241126-0c182b82-6619-47e3-bfa6-88b5a3b7b2c4.PNG)

Full adder:
![RTL realization](https://user-images.githubusercontent.com/94154683/164241126-0c182b82-6619-47e3-bfa6-88b5a3b7b2c4.PNG)



### Result:
Thus,the Implementation of Half Adder and Full Adder circuit are studied and the truth table for different logic gates are verified.
