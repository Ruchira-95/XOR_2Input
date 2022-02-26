# XOR Gate Using CMOS 28nm Technology
Implementation of 2 input XOR gate using CMOS 28nm technology.

**Abstract**:- The scope of the work is to design a two input XOR gate using 28nm CMOS. Exclusive OR (XOR) gate is utilized in various digital system applications such as full adder, comparator, parity checker and controlled inverter.

Keywords- XOR, CMOS


*1. Introduction*

XOR gates have many application in digital systems. Hence it is necessary to implement these gates for their various applications. Implementing circuits using only universal gates will increase the number of gates used thus we need to use basic gates to reduce the number of gates in the circuit.

A MOSFET has 4 terminals drain, gate, source and substrate. CMOS means Complementary Metal Oxide Semiconductor. The CMOS Transistor is constructed by both NMOS and PMOS Transistors. It is basically an integrated circuit built with those two transistors. As both the transistors are used, the CMOS has both characteristics. The NMOS transistors in the CMOS creates a low resistance path between the source and drain when the gate voltage is high and the PMOS transistor in the CMOS creates a low resistance path between the source and drain when the gate voltage is low. [1]

*2. Circuit Design*

A XOR gate can be implemented using 10 MOSFETs, 5 NMOS and 5 PMOS each.

![Logical Block Diagram of XOR Gate](Xor.png) 

![Truth Table](XORTT.png)

From the truth table of the XOR gate, the output is high only when the two inputs are not equal thus it represents an inequality function. The above logic block diagram shows the implementation of XOR gate using 2 NOR and 1 AND gate. The same can be implemented using CMOS. 

![CMOS XOR](CMOS%20XOR.png)

MOSFETs Q1, Q2, Q3, and Q4 form the NOR gate. Q5 and Q6 do the ANDing of A and B, while Q7 performs the ORing of the NOR and AND outputs.  Q8, Q9, and Q10 complement the assembly of Q5, Q6, and Q7, inverting the output. [2]

*3. Waveform*

The output of XOR gate is high only if the given two inputs are unequal. If A and B are the inputs to XOR gate then the output is high only if A is low, B is high or A is high, B is low.

![XOR](XOR%20Wave.png)

*4. Result and Output Waveform*

![XOR Synopsys](cp_lib1_XOR_schematic2.jpeg)
