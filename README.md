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
/*
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: Lokesh N
RegisterNumber:  22008481

Half adder program:

module halfadd (a,b,sum,carry);

input a,b;

output sum,carry;

assign sum = (a^b);

assign carry = (a&b);

endmodule

Full adder program:

module fulladd (a,b,c,sum,carry);

input a,b,c;

output sum,carry;

assign sum = (a^b^c);

assign carry = ((a&b)|(a^b)&c);

endmodule  
*/
Logic symbol & Truthtable
RTL realization

### Output:
### RTL
![image](https://user-images.githubusercontent.com/119393019/213872889-760cde09-ab04-46ff-b3bf-c9f00cca27aa.png)
![image](https://user-images.githubusercontent.com/119393019/213872903-2ba80c0d-06dd-450b-aadd-f862dc78955f.png)

### TIMING DIAGRAM
![image](https://user-images.githubusercontent.com/119393019/213872947-7ccfe577-44ec-4b80-a3c0-60ce1702c6f3.png)
![image](https://user-images.githubusercontent.com/119393019/213872985-dc206417-0674-4ffb-af4f-35b783fd1ace.png)


### TRUTH TABLE 
![image](https://user-images.githubusercontent.com/119393019/213873012-8fda6e0e-c79c-4d26-8da3-20d6e93c2c9f.png)

![image](https://user-images.githubusercontent.com/119393019/213873032-ff5e7a81-e7a7-48f5-bc69-c551daff0326.png)

### Result:
Thus the Implementation of Half Adder and Full Adder circuit are studied and the truth table for different logic gates are verified.
