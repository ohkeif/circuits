# Quad Drone Keychain



![CKACB](https://github.com/ohkeif/circuits/blob/main/Common_Circuits/Quad_Drone_2025/Quad_Drone/images/pcb.png)

(Note: the 18v silkscreen indicator is placed where the GND wire should go! Be sure the GND goes into the square terminal and power goes into the circular one).



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

This circuit is based off the Look Mum No Computer's oscillator circuit, but ramped up to 11...or 4 I guess. With 4 CV compatible oscillators, this circit is capable of producing a variety of hypnotic harmonically rich soundscapes. Each oscillator is selectable using a corresponding swtich, allowing for 24 combinations of stacking and building sounds. Start with a single drone or dial in a massive 4 note chord with step sequenced CV inputs to turn the drone into a lo-fi synth that stays perfectly in time with other instruments. The circuit consists of four 2n3904 transistors and an assortment of resistors and capacitors. In operation, the value of the capacitors and LEDs determine the frequency range of the resulting sounds. Mix and match capacitor values and LED colors to personalize your drones to taste to unleash a menagerie of mesmerizing meditative melodies. 

## Assembly Instructions
Organize all your components to match up with the BOM to ensure you have everything you need to get started! Begin placing all the components onto the top side of the board with their legs poking through to the other side. 

* R1-R4 are 1k ohm resistors with the color code: Brown, Black, Red. These acts as a current limiter for the LEDs. 
* R5-R8 are 100k ohm resistors (Brown, Black, Yellow). These act as a rudimentary mixer to avoid cross-talk of the 4 oscilators. 
* Frequency controls are made from the interaction of the transistor operating in reverse avalanche mode. Each oscillator can be tuned using a 10k potentiometer and expermimenting with different values of LED/Capacitor/Transistor
* SPST switches are used to toggle each oscillator on or off


Once all components are placed on the board, tape down (or otherwise secure) all the components and flip over the board to solder everything up! 



### Electrolytic Capacitor Polarity
This board uses electrolytic capacitors - the ones with a cylindrical shape. These capacitors are polarized, meaning they have a positive and negative side. The negative is identifiable from the white stripe along one side. This stripe should line up with the white markings on the PCB silkscreen. 

![Polar Caps](https://github.com/ohkeif/circuits/blob/main/Common_Circuits/Atari_Punk_Console_2024/images/polar_caps.png)




### Schematic
![schematic](https://github.com/ohkeif/circuits/blob/main/Common_Circuits/Quad_Drone_2025/Quad_Drone/images/schematic.png)
