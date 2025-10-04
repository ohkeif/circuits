# Quad Drone Keychain


## What Dis Do?



![CKACB](https://github.com/ohkeif/circuits/blob/main/Common_Circuits/Quad_Drone_2025/Quad_Drone/images/pcb.png)
## But, I am not a Circuit Builder

Do not worry yourself with temporary concerns. And until you start on your learning journey, the CKACB will serve as a stylish keepsake of a truly memorable and life changing event for you. 


## BOM (Bill of Materials)

| Qty              | Reference | Value |
| :---------------- | :------: | ----: |
| 2	|C1, C2	             | 10uf|
|1	|C3|	4.7uf|
|1	|C4	|2.2uf|
|4	|D1, D2, D3, D4	|LED|
|4	|FREQ1-4|	10k Linear|
|1	|PWR	|18v DC IN|
|1	|OUT	|Audio Out
|4	|R1, R2, R3, R4	|1K|
|4	|R5, R6, R7, R8	|100K|
|4	|Q1, Q2, Q3, Q4	|2n3904|
|4	|SW1, SW2, SW3, SW4	|SPST|


## Quadruple Oscillators

This circuit is based off the Look Mum No Computer simple oscillator circuit. It bleeps, bloops, and otherwise generates 8-bit console sounds. Sounds like high pitched zipping lasers and spacey distorted rocket arcade engine sounds. The circuit consists of two of the ubiquitous 8-pin DIP IC, the 555 timer, and an assortment of resistors and capacitors. In operation, the first timer is wired as an astable multivibrator that acts as a frequency oscillator. The second is set up as a monostable multivibrator that acts as the pulse width modulation of the firs timer. In other words, the oscillator (555 timer 1) drives the monostable (555 timer 2), which emits square output pulses with a duration controlled by the pulse width potentiometer. The resulting stepped tones almost sound like magic as they jump through lo-fi notes similar to chromatic rising and falling of keys on a keyboard.

## Assembly Instructions
Organize all your components to match up with the BOM to ensure you have everything you need to get started! Begin placing all the components onto the top side of the board with their legs poking through to the other side. 

Looking at the capacitors, C1 is marked with "103", where C2 is marked with "104". These numbers equate to the capacitance values, 0.01uf and 0.1uf respectively. 
C3 is an electrolytic capacitor with a cylindrical shape. This capacitor is polarized, meaning it has a positive and negative side. Find the negative side with the white stripe and place it accordingly on the board. 

### Electrolytic Capacitor Polarity
![Polar Caps](https://github.com/ohkeif/circuits/blob/main/Common_Circuits/images/polar_caps.png)


R1 and R2 are both 1k ohm resistors with the color code: Brown, Black, Red. R1 acts as a current limiter for the LED. R2 and the Frequency potentiometer controls the frequency of the audio oscillator. R3 and R4 along with the 10uf electrolytic capacitor form a low-pass filter that cut's high end artifacts from the audio output. Pulse Width controls the output pulse duration of the monostable multivibrator. And it is possible to add a mono jack onto pin 5 of each 555 chip to enable CV (control voltage) inputs for both controls.

Solder the IC socket with the correct orientation onto the board. Keep note of the notch on one end. Insert the IC into the IC socket staying consistent with the notch. Or don't use a socket. Just be careful and give the chip some time to cool off between soldering pins if soldering sans socket. 


### IC and IC Socket
![IC and IC Socket](https://github.com/ohkeif/circuits/blob/main/Common_Circuits/images/dip-orientation.jpg)

Finally, obtain some spools of wire (20-24 gauge stranded core) and wire up the potentiometers, switches and power connections. To keep things organized, it may help to use green wire for ground connections, red wire for 9v connections, and yellow wire for audio connections. 


Now you can tape down all the components and flip over the board to solder everything up! 


### Schematic
![schematic](https://github.com/ohkeif/circuits/blob/main/Common_Circuits/images/schematic.png)
