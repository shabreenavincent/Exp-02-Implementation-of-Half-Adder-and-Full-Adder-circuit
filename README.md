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
### 
Program:

HALF ADDER

/*
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.


HALF ADDER  

module HalfAdder(a,b,sum,carry);
input a,b;
output sum,carry;
xor(sum,a,b);
and(carry,a,b);
endmodule  

FULL ADDER  

module FullAdder(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum = ((a^b)^c);
assign carry = ((a&b)|(b&c)|(c&a));
endmodule 



Developed by: Shabreena Vincent
RegisterNumber: 22009378 
*/
Logic symbol 



![logic gates](https://user-images.githubusercontent.com/119475721/212956724-82078ce3-da3f-430b-a7aa-11ba93891ada.png)


RTL realization

 Output:
half adder





![half adder output](https://user-images.githubusercontent.com/119475721/212956948-c7d2e7f2-6169-4094-bae8-ec5f5e197ee9.png)



full adder





![full adder output](https://user-images.githubusercontent.com/119475721/212955934-99bfa51d-2651-42d3-bdb6-931f3ec59e67.png)



 RTL TIMING DIAGRAM

half adder




![rtl timing diagram half adder](https://user-images.githubusercontent.com/119475721/212955976-138fbfb2-0950-4d77-89be-5716bd855fe8.png)

full adder




![rtl timing diagram full adder](https://user-images.githubusercontent.com/119475721/212956001-8099af7c-df33-4c8a-9daf-5f7d5dbe3e87.png)


TRUTH TABLE 


half adder




![truth table half adder](https://user-images.githubusercontent.com/119475721/212956182-9860a677-17e6-44b3-81d7-13a0851a1b1d.png)


full adder




![truth table full adder](https://user-images.githubusercontent.com/119475721/212956207-b31a103e-7acf-4fdc-9590-d053dbdb9652.png)



 Result:
 Thus the Implementation of Halfadder Fulladder Circuit are studied and the truthtable for different logic gates are verified
