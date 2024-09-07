# Verilog-Voting-Machine


## Overview
In this project, voting machine is implemented using the Verilog hardware description language (HDL) to create a digital voting machine.

## Flowchart
![flowchart](https://github.com/Anuagra24/Electronic-Voting-Machine/assets/98021398/3be87721-245b-4088-9e2d-e78c6ebd916a)

## Components
This project contains four verilog modules:-
1. Button Control module
2. Mode Control module
3. Vote Logger module
4. Voting Machine module

### Software Used:- EDA Playground

Hardware:-Diligent Zedboard(Zynq-7000 SoC)

## Output of EPwave Waveform
![WhatsApp Image 2024-03-30 at 02 50 32_15475c06](https://github.com/Anuagra24/Electronic-Voting-Machine/assets/98021398/0a86759a-6acf-4d0e-be45-609b74c08720)


## Brief Description of the modules:

### 1. Button Control Module
This module is responsible for detecting and managing inputs.It includes functionality for debouncing (eliminating bouncing effect caused by mechanical contacts) to ensure accurate button press detection.

a)The vote should be logged only after the button has been pressed for a certain amount of time.

b) Only a single vote should be logged if button is pressed for a large duration.

### 2.Mode Control Module
The mode control module manages the different modes of operation of the voting machine, such as setup mode, voting mode, and result display mode.

During the voting mode, it enables voters to cast their votes accurately.

After the voting period, it switches to the result display mode to show the outcome of the voting process.

a)It is used for control of LEDs.

b)For voting mode, LEDs light up for a second to indicate the vote has been cast.

c)For tally mode, the LEDs light up in binary numbers to indicate the number of votes received by the candidate.

### 3. Vote Logger Module
This module is responsible for logging the votes cast by the voters.

a) Logs the valid votes only if it is in the proper mode.

b) Also used to reset the values at the start of operation.

### 4.Main Voting Machine module
This module acts as the core component of the voting machine, integrating the functionalities of button control, mode control, and vote logging.
It coordinates the interactions between the different modules based on the current mode of operation.
