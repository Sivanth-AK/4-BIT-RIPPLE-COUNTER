<img width="1600" height="847" alt="image" src="https://github.com/user-attachments/assets/8f9f710b-1f7e-4401-9de6-84fafeaab609" /># 4-BIT-RIPPLE-COUNTER

**AIM:**

To implement  4 Bit Ripple Counter using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

**4 Bit Ripple Counter**

A binary ripple counter consists of a series connection of complementing flip-flops (T or JK type), with the output of each flip-flop connected to the Clock Pulse input of the next higher-order flip-flop. The flip-flop holding the least significant bit receives the incoming count pulses. The diagram of a 4-bit binary ripple counter is shown in Fig. below.

![image](https://github.com/naavaneetha/4-BIT-RIPPLE-COUNTER/assets/154305477/cb4b74d4-31ab-4359-95d0-d22e67daba13)

In timing diagram Q0 is changing as soon as the negative edge of clock pulse is encountered, Q1 is changing when negative edge of Q0 is encountered(because Q0 is like clock pulse for second flip flop) and so on.

![image](https://github.com/naavaneetha/4-BIT-RIPPLE-COUNTER/assets/154305477/a573a7d6-014e-4e54-93e6-e2ac9530960b)

![image](https://github.com/naavaneetha/4-BIT-RIPPLE-COUNTER/assets/154305477/85e1958a-2fc1-49bb-9a9f-d58ccbf3663c)

**Procedure**

/* write all the steps invloved */

**PROGRAM**

/* Program for 4 Bit Ripple Counter and verify its truth table in quartus using Verilog programming.

 Developed by:Sivanth T RegisterNumber:212225240150
*/
module ripple_counter(clk,rst,t,A,B,C,D); 
input clk,rst,t; 
output A,B,C,D;
reg A,B,C,D;

Tff T0(D,clk,rst,t); 
Tff T1(C,D,rst,t); 
Tff T2(B,C,rst,t); 
Tff T3(A,B,rst,t); 

endmodule 


**RTL LOGIC FOR 4 Bit Ripple Counter**
[RTL pdf (4).pdf](https://github.com/user-attachments/files/26203850/RTL.pdf.4.pdf)


**TIMING DIGRAMS FOR 4 Bit Ripple Counter**
<img width="1600" height="847" alt="image" src="https://github.com/user-attachments/assets/881ae033-1ee1-4ef2-b934-436cacb4ef00" />

**RESULTS**
 4 Bit Ripple Counter using verilog and validating their functionality using their functional tables is implemented
