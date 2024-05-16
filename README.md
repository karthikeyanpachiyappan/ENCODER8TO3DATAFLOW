## EX-11 <p align="center"><b> ENCODER8TO3DATAFLOW </b>    

**DATE:**


**AIM:**

To implement  Encoder 8 To 3 in Dataflow Modelling using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:** Quartus prime

**THEORY**

**Encoder 8 To 3**

The 8 to 3 line Encoder is also known as Octal to Binary Encoder. In 8 to 3 line encoder, there is a total of eight inputs, i.e., D0, D1, D2, D3, D4, D5, D6, and D7 and three outputs, i.e., A0, A1, and A2. In 8-input lines, one input-line is set to true at a time to get the respective binary code in the output side. Below are the block diagram and the truth table of the 8 to 3 line encoder.

![image](https://github.com/karthikeyanpachiyappan/ENCODER8TO3DATAFLOW/assets/155143878/908b0da5-aef2-4d70-b1e6-9674a68e3039)


Figure 01  Block Diagram of Encoder 8 * 3

**Truth Table**

![image](https://github.com/karthikeyanpachiyappan/ENCODER8TO3DATAFLOW/assets/155143878/86387a85-c42a-48a1-9269-6f9aa0b37d39)


The logical expression of the term A0, A1, and A2 are as follows:

A0 = D1 + D3 + D5 + D7

A1 = D2 + D3 + D6 + D7

A2 = D4 + D5 + D6 + D7

Logical circuit of the above expressions is given below:

![image](https://github.com/karthikeyanpachiyappan/ENCODER8TO3DATAFLOW/assets/155143878/7a4622d0-cae4-40f6-a2dc-d3caa03bfc2d)


Figure 02  Encoder 8 * 3

**Procedure**

```
1.Type the program in Quartus software.

2.Compile and run the program.

3.Generate the RTL schematic and save the logic diagram.

4.Create nodes for inputs and outputs to generate the timing diagram.

5.For different input combinations generate the timing diagram
```

**PROGRAM**

**Developed by: KARTHIKEYAN P**

**RegisterNumber:212223230102**

```
module encoder(a0,a1,a2,d0,d1,d2,d3,d4,d5,d6,d7);
input d0,d1,d2,d3,d4,d5,d6,d7;
output a0,a1,a2;
//add logic here using dataflow modelling
assign a0=d1|d3|d5|d7;
assign a1=d2|d3|d6|d7;
assign a2=d4|d5|d6|d7;
endmodule
```
**RTL LOGIC FOR Encoder 8 To 3 in Dataflow Modelling**

![image](https://github.com/karthikeyanpachiyappan/ENCODER8TO3DATAFLOW/assets/155143878/2598da16-f0b3-4004-afab-4a140df2275c)


**TIMING DIGRAMS FOR Encoder 8 To 3 in Dataflow Modelling**

![image](https://github.com/karthikeyanpachiyappan/ENCODER8TO3DATAFLOW/assets/155143878/15d8d340-e6cc-4ea1-b63e-bcd75b9d4d33)


**RESULTS**

Thus,the Encoder 8 To 3 in Dataflow Modelling using verilog has been implemented successfully and their functionality is validated using their functional tables.



