# Exp-03-Implementation-of-Half-Adder-and-Full-Adder-circuit

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

```
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: HARISH RAGAVENDRAS
RegisterNumber:  212222230045
```

Half adder program:
```
module fulladd (a,b,sum,carry);
input a,b;
output sum,carry;
assign sum = (a^b);
assign carry = (a&b);
endmodule
```
Full adder program:
```
module fulladd (a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum = (a^b^c);
assign carry = ((a&b)|(a^b)&c);
endmodule
```
Logic symbol & Truthtable
RTL realization

### Output:

### RTL
## HALF ADDER:
![rtl ex 3](https://user-images.githubusercontent.com/114852180/231665254-a2c28d40-7df8-4fa4-9cb0-1f6fa15cac04.png)

## FULL ADDER:
![fulladder rtl](https://user-images.githubusercontent.com/114852180/231665594-3d0e91eb-84e2-4b4f-9763-f252bd8fae64.png)

## TIMING DIAGRAM:

## HALF ADDER:
![waveform ex3](https://user-images.githubusercontent.com/114852180/231665765-851f552d-8acb-451a-aa9b-5075878c1562.png)
## FULL ADDER:
![ex 03 waveform full adder](https://user-images.githubusercontent.com/114852180/231665808-5ae81da8-f8ed-4343-bf79-17092fc7eb94.png)

### TRUTH TABLE:
## HALF ADDER TRUTH TABLE:
![halfadder truth table](https://user-images.githubusercontent.com/114852180/231666115-5e51980a-76f9-4d1d-b708-0c01e0db7792.png)

## FULL ADDER TRUTH TABLE:
![Screenshot 2023-04-13 112441](https://user-images.githubusercontent.com/114852180/231666448-d3885304-3962-46b6-84f0-bdd2142c909c.png)




### Result:
Thus the Implementation of Half Adder and Full Adder circuit are studied and the truth table for different logic gates are verified.
