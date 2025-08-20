Key Components

Arduino Nano: The microcontroller that serves as the brain of the circuit, storing the code for the traffic light sequence and countdown logic.

74HC595 Shift Registers: Three shift registers are used to expand the number of output pins from the Arduino. This allows the single microcontroller to control all the LEDs and 7-segment displays without needing a dedicated pin for each.

Red, Yellow, and Green LEDs: These LEDs represent the traffic lights. They are controlled by transistors which act as switches to handle the necessary current.

7-Segment Displays: Two displays are used to show the countdown timer. They are controlled by the shift registers to display numbers from 99 down to 0.

Transistors: Used to amplify the current from the shift registers to power the LEDs and 7-segment displays.

How It Works
The Arduino Nano is programmed with the timing logic for the traffic lights. Instead of using a dedicated digital pin for each of the LEDs and 7-segment display segments, the Arduino sends data to the shift registers. These registers then "shift" the data out to their individual output pins, effectively acting as pin multipliers. This allows the Arduino to manage a large number of outputs with a minimal number of connections.

The transistors act as switches, turning the LEDs on and off according to the signals from the shift registers. The 7-segment displays receive data to show the time remaining before the light changes.
