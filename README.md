# FULL_ADDER_SUBTRACTOR

Implementation-of-Full-Adder-and-Full-subtractor-circuit

**AIM:**

To design a Full Adder and Full Subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime

**Full Adder and Full Subtractor**

**Full Adder**

Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin 

Carry = AB + ACin + BCin

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/0f30ba51-5ffb-4198-845f-18e054f675e7)

**Figure -1 FULL ADDER**

**Full Subtractor**

A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow.

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/02b24f51-ab51-4304-9ad6-7b81ffc1ead5)

Diff = A ⊕ B ⊕ Bin 

Borrow out = A'Bin + A'B + BBin

**Truthtable**

<img width="334" height="234" alt="image" src="https://github.com/user-attachments/assets/9b7daf6b-0648-4eb1-8ac5-586a61e70522" />

<img width="299" height="234" alt="image" src="https://github.com/user-attachments/assets/4cef069e-e8b6-4019-b99b-d5bebd13e35e" />

**Procedure**

1.Type the program in Quartus software.

2.Compile and run the program.

3.Generate the RTL schematic and save the logic diagram.

4.Create nodes for inputs and outputs to generate the timing diagram.

5.For different input combinations generate the timing diagram.

**Program:**

/* Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming. 
```
module EX4(a,b,c,d,e,f,sum,car,diff,borr);
input a,b,c,d,e,f;
output sum,car,diff,borr;
assign sum = a^b^c;
assign car = a&b|a&c|b&c;
assign diff = d^e^f; 
assign borr = (~d&f)|(~d&e)|(d&e);
endmodule

```
Developed by: RITHIKA.K

RegisterNumber: 25017528

*/

**RTL Schematic**
<img width="1920" height="1080" alt="Screenshot 2025-11-20 145946" src="https://github.com/user-attachments/assets/98cff283-4f01-49c9-87c0-86709fdaf56d" />

**Output Timing Waveform**
<img width="1920" height="1080" alt="Screenshot 2025-11-20 183754" src="https://github.com/user-attachments/assets/d5390656-4ca5-40db-b3d5-66b397cd44c3" />

**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



