
# EEMP Digital Design Lab
<img src="assets/images/DigitalDesignLabHeader.png" style="margin-top: 0">
<p style="text-align:center;">Welcome to the EEMP Digital Design Laboratory!</p>

# Background
All the electronics around you can be decomposed to binary, ones and zeros. For example, the very device that you are using to look at this page is being translated to ones and zeros for your display controller (HDMI) to show. 

Examples: 
- Controllers
- Logic (Algorithms)
- PWM Signals for controlling servos
- Communication
- Computer Architecture 

In this lab, you will look at various signals and get a feel of how looking at signals can allow you to get a "feel" about how computers work. 


## Signals
![Square Wave](assets/images/square_wave.png)
(Figure x. Square Wave)

A **signal** is a square wave function that represents binary values of a high (1) and low value (0). Square waves have characteristics such as frequency and duty cycle. Frequency (Hz) is defined as how often the wave repeats itself per second. Knowing the frequency is important since it is used in sequential logic and determines how fast the digital design can run. 
Duty cycle is the ratio between how long the signal stays high versus low. Duty cycle is important in applications like turning a wheel as controlliI needng the duty cycle controls how fast or slow the wheel would move. 
Square waves can be generated through various means such as natural crystals, analog circuit components, and even digital design itself. 


## Combinational Logic
![Combinational Logic](assets/images/combinational_logic.png)
(Figure x. Combinational Logic)
![Combinational Logic Truth Table](assets/images/truth_tables.png)
(Figure x. Combinational Logic Truth Table)

Recall from the lecture about logic gates where AND, OR, NOT, XOR gates allow you to make calculations and decisions. 
Combinational Logic is a type of signal where the output only depends on the current input values. The figures above are the truth tables to common logic gates.


## Sequential Logic 
![Sequential Logic](assets/images/sequential_logic.png)
(Figure x. Sequential Logic)
Sequential Logic is a type of signal where the output depends on both the current value and the sequence of past inputs. 
Sequential Logic allow signals to have memory about past decisions. One example is having a counter that counts upwards or downwards. 

## Binary<->Hexadecimal<->ASCII Conversion
In the context of digital design, binary is the most fundamental unit but often times converting to other units allow you to look at information more easily. 
Converting binary to hexadecimal allows you to reduce the number of visible digits there are. Then converting hexadecimal to ASCII is as easy as looking at the **two** hexadecimal values. The table below shows binary to its respective hexadecimal value. 

Binary to Hexadecimal Table:
| Binary | Hexadecimal | 
| ------ | ----------- |
| 0000   |      0      |
| 0001   |      1      |
| 0010   |      2      |
| 0011   |      3      |
| 0100   |      4      |
| 0101   |      5      |
| 0110   |      6      |
| 0111   |      7      |
| 1000   |      8      |
| 1001   |      9      |
| 1010   |      A      |
| 1011   |      B      |
| 1100   |      C      |
| 1101   |      D      |
| 1110   |      E      |
| 1111   |      F      |

(Ex. Convert 0b1100_1101_0011_0001 = 0xCD31) 
Tip: By splitting the bits into segments of 4 bits, converting it into hexadecimal is now just matching the 4 bits to its respective hexadecimal value. 

 
![Ascii Table](assets/images/ascii_table.png)
(Figure x. ASCII Table)

## Simulation
- Square Wave simulation showcase 
- How to look at the waveforms

# Instructions

## Setup
- Download git - https://git-scm.com/downloads
    - If you are using windows, downloading from git-scm.com will give you a program called "Git Bash" 
    - If you are using mac, you can download via `brew install git` using homebrew and check that it has been installed 
    `git -v`
- Clone this repository
    - In git bash or your respective shell, execute this command: 
    `git clone https://github.com/Science-Mentorship-Institute/eemp_digital_design.git`
    - Alternatively: Download the files directly
        - Go to https://github.com/Science-Mentorship-Institute/eemp_digital_design.git
            - Press the Green "Code" Button and then click "Download ZIP"
            - Extract the ZIP to retrieve the files 

## Surfer Waveform Viewer Overview
Surfer Waveform Viewer Online: https://app.surfer-project.org/
- Surfer can be installed locally. See: https://gitlab.com/surfer-project/surfer

The figure below shows the surfer user interface. 

![Surfer Waveform Viewer Overview](assets/images/surfer_overview.png)

# Lab 0: Warmup
Drawing truth tables for combinational logic on a canvas quiz.

# Lab 1
Message Translation 
Open `lab1_message_wave.vcd` file in a waveform viewer. 

Decode the message and write the code in ASCII Here: ____ 

# Lab 2
RISC Instruction Translation

Open `lab2_instruction_wave.vcd` file in a waveform viewer. 

Decode the RISC Instruction and write the instruction here (format: TODO): ____ 

# Lab 3
Traffic Lights 

Open `lab2_traffic_light_wave.vcd` file in a waveform viewer. 

Figure out the sequence that the traffic lights is on and various attributes of the traffic lights.
How much CLK cycles does the green light stay on for? 
How much CLK cycles does the orange light stay on for? 
How much CLK cycles does the red light stay on for? 
TODO.. Some more questions

# Lab 4 
Protocols and Communication
UART Waveform and Translation
TODO.

# Lab 5
?? 



# (Optional)

## Generating the Waveforms
- Using RTL language and simulation 
[Click Here for more information about generating waveforms.](assets/Generating_Wave_Forms.md)

## Non-Ideal Conditions
A square wave is never just a square wave, in a real world, the square wave will slew due to many factors. 

![Square wave Slewing](assets/images/square_wave_slewed.png)
(Figure x. Square Wave Slewing)

[Click Here for more information about non ideal conditions](assets/Non_Ideal_Conditions.md)

<img src="assets/images/sinewave_to_squarewave.jpg" width="1200" height="700">
(Figure x. Sine wave to Square Wave)

## Alternative Waveform Viewer: GTKWave
- see: https://gtkwave.sourceforge.net

