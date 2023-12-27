# Experiment--03-Half-Subtractor-and-Full-subtractor
## Implementation-of-Half-subtractor-and-Full-subtractor-circuit
## AIM:
To design a half subtractor and full subtractor circuit and verify its truth table in Quartus using Verilog programming.

## Equipments Required:
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime
## Theory
Subtractor circuits take two binary numbers as input and subtract one binary number input from the other binary number input. Similar to adders, it gives out two outputs, difference and borrow (carry-in the case of Adder). There are two types of subtractors.

## Half Subtractor Full Subtractor
## Half Subtractor
The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed.
![half-subtractor9]!![image](https://github.com/23008344/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/145742655/925408e0-7a14-4e1c-ba17-5b90580e8d6e)



Sum = X'Y+XY' = X ⊕ Y
Carry=X'Y

## Full Subtractor
A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow. 
![full-subtractor6]!![image](https://github.com/23008344/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/145742655/9dd6f352-198f-4c17-84dc-56802c81d04a)



Diff = A ⊕ B ⊕ Bin B = A'Bin + A'B + BBin

## Procedure

1.	Create a New Project:

      Open Quartus and create a new project by selecting "File" > "New Project Wizard."
 
      Follow the wizard's instructions to set up your project, including specifying the project name, location, and target device (FPGA).

2.	Create a New Design File:

    Once the project is created, right-click on the project name in the Project Navigator and select "Add New File."
     Choose "Verilog HDL File" or "VHDL File," depending on your chosen hardware description
     language.

3.	Write the Combinational Logic Code:

      Open the newly created Verilog or VHDL file and write the code for your combinational logic.

4.	Compile the Project:

     To compile the project, click on "Processing" > "Start Compilation" in the menu.
     Quartus will analyze your code, synthesize it into a netlist, and perform optimizations based on your target FPGA device.

5.	Analyze and Fix Errors:

    If there are any errors or warnings during the compilation process, Quartus will display them in the Messages window.
    Review and fix any issues in your code if necessary. View the RTL diagram.

6.	Verification:

    Click on "File" > "New" > "Verification/Debugging Files" > "University Program VWF".
    Once Waveform is created Right Click on the Input/Output Panel > " Insert Node or Bus" > Click on Node Finder > Click On "List" > Select All.
    Give the Input Combinations according to the Truth Table amd then simulate the
    Output Waveform.





## Program:
/*
Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming.

Developed by: VARNIKA.P

RegisterNumber:  23008344
*/

## Half Subractor:

![image](https://github.com/23008344/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/145742655/a979b968-00b1-4c87-99a0-5000b4a48812)



## Full Subractor:

![image](https://github.com/23008344/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/145742655/5ee7f32e-8a8f-46c6-b157-068b2cceb40b)




## Truthtable

## HALF SUBTRACTOR 

![image](https://github.com/23008344/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/145742655/33732ac1-be4c-4ca3-85da-ab6a70ace855)


## FULL SUBTRACTOR

![image](https://github.com/23008344/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/145742655/303150de-c440-4e10-b352-2d687f25a995)


##  RTL realization

## HALF SUBTRACTOR 

![image](https://github.com/23008344/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/145742655/7b72d9a6-53d6-4b9d-ba73-13e12c83e580)


## FULL SUBTRACTOR

![image](https://github.com/23008344/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/145742655/e9877e19-28d3-42cc-8e6e-344f70ad2746)


## Timing diagram 

## HALF SUBTRACTOR 

![image](https://github.com/23008344/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/145742655/f4708437-2ea7-45a5-aa5a-fba154ff2a25)


## FULL SUBTRACTOR

![image](https://github.com/23008344/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/145742655/1a31ac8e-f843-4a2e-aafa-510f7792da47)


## Result:
Thus the half subtractor and full subtractor circuits are designed and the truth tables is verified using quartus software.
