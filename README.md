7-Segment Display Control with Arduino UNO
In this project, you will learn how to interface and program a 7-segment display using an Arduino UNO. You'll display digits by selectively turning on the segments of the display, allowing you to show numbers like a digital clock or calculator.

📦 Components Required
1 × Arduino UNO

1 × USB Cable

1 × 7-Segment Display (Common Cathode or Common Anode)

1 × 220Ω Resistor

1 × Breadboard

Several Jumper Wires

🧠 Principle
A 7-segment display is made up of eight LEDs arranged to form the number “8”. Each segment (labeled a to g, and dp for decimal point) can be turned on or off to create digits from 0 to 9.

There are two types of displays:

Common Cathode (CC): Common pin goes to GND

Common Anode (CA): Common pin goes to VCC

Each segment is lit by sending a HIGH or LOW signal depending on the display type.

Segment Map
Digit	Segments On
0	a, b, c, d, e, f
1	b, c
2	a, b, g, e, d
3	a, b, g, c, d
4	f, g, b, c
5	a, f, g, c, d
6	a, f, e, d, c, g
7	a, b, c
8	all segments (a-g)
9	a, b, c, d, f, g

🔌 Wiring (Example for Common Cathode)
Segment	Arduino Pin
a	2
b	3
c	4
d	5
e	6
f	7
g	8
dp	(optional)
COM	GND

Use a 220Ω resistor between each Arduino pin and its corresponding segment.

Connect COM pin to GND (for common cathode).


📸 Output
The 7-segment display will show digits 0 through 9, each for 1 second, in a continuous loop.
