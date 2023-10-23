# Water-Leakage-Detection-Module-1

This project is about detecting leaks in water pipes using two flow sensors, a solenoid valve, an Arduino Uno, a relay kit, and an LED and buzzer.

## Components

- Two flow sensors: These are devices that measure the rate of flow of water in liters per minute. They are connected to the pipe at both ends of each branch
- A solenoid valve: This is an electrically operated valve that can open or close the pipe. It is connected to the relay kit using wires.
- An Arduino Uno: This is a microcontroller board that can read inputs from sensors and control outputs such as relays, LEDs, and buzzers. It is programmed using the Arduino IDE software.
- A relay kit: This is a module that can switch high-voltage or high-current devices using low-voltage or low-current signals from the Arduino Uno.
- An LED and buzzer: These are simple devices that can produce light and sound respectively. They are connected to the Arduino Uno using resistors and wires.

## Working Principle

- The Arduino Uno reads the flow rate values from the two flow sensors using analog pins 2 and 3. It moniters them using a formula based on the specifications of the sensors.
- The Arduino Uno compares the two flow rate values and calculates the difference. If the difference is greater than a threshold value (which can be adjusted in the code), it means that there is a leak in the pipe.
- The Arduino Uno then sends a HIGH signal to pin 6, which is connected to the relay kit. The relay kit switches on the solenoid valve, which closes the pipe and stops the water flow.
- The Arduino Uno also sends HIGH signals to pins 4 and 5, which are connected to the LED and buzzer respectively. The LED turns on and the buzzer beeps to indicate that there is a leak.
- The user can then inspect the pipe and fix the leak.
- Once the leak has been corrected the arduino opens the solenoid valve to resume the flow.

## Installation

To install this project, you need to have the following software and hardware:

- Arduino IDE: This is the software that allows you to write and upload code to your Arduino board. You can download it from [here](https://www.arduino.cc/en/software).
- Flow sensors
- Solenoid valve
- Arduino Uno
- Relay kit
- LED and buzzer

To install this project, follow these steps:

1. Connect the flow sensors to the pipe at both ends . Make sure they are aligned with the direction of water flow.
2. Connect the solenoid valve to the pipe near the water source and also to arduino using wires.
3. Connect the relay kit to the solenoid valve using wires. Make sure you connect them to the correct terminals according to the relay kit manual.
4. Connect the Arduino Uno to your computer using a USB cable.
5. Open the Arduino IDE and select your board type and port number from the Tools menu.
6. Download into your Arduino IDE.
7. Upload the code to your Arduino board by clicking on the Upload button.
8. Connect the LED and buzzer to pins 9 and 10 of your Arduino board using resistors and wires.
9. Test your project by turning on the water supply and creating a leak in your pipe.

## Usage

To use this project, you need to monitor your LED and buzzer for any signs of leakage. If you see or hear them, the arduino closes the solenoid valve and stops the water supply. When the leak has been corrected the arduino again opens the solenoid valve and resumes the supply
