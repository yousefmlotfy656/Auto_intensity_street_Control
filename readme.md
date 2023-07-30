Auto Intensity Control of Street Lights using Arduino
The Auto Intensity Control of Street Lights using Arduino is a smart project that automatically adjusts the brightness of street lights based on ambient lighting conditions. This project utilizes an Arduino board, an RTC Module (DS3231), an LDR (Light Dependent Resistor), and LEDs for street lights.

Concept
The main idea behind this project is to save power by controlling the street lights' intensity. There are two modes of operation: RTC Mode and LDR Mode.

RTC Mode: In this mode, the street lights automatically turn on at the specified ON time and turn off at the specified OFF time, which can be set in the Arduino code.

LDR Mode: In this mode, the street lights' intensity is adjusted based on the ambient light detected by the LDR. As the surrounding light changes, the intensity of the LEDs changes accordingly.

Circuit Diagram
The circuit diagram of the Auto Intensity Control of Street Lights using Arduino project is as follows:

Circuit Diagram

Components Required
Arduino UNO
DS3231 RTC Module
LDR (Light Dependent Resistor)
16x2 LCD Display
LEDs (for street lights)
10KΩ Potentiometer
10KΩ Resistor
Push Button
Connecting Wires
Breadboard
Circuit Design
Connect the SDA and SCL pins of the DS3231 RTC Module to A4 (SDA) and A5 (SCL) pins of the Arduino.

Create a voltage divider using a 10KΩ resistor and an LDR. Connect the output of the voltage divider to A3 pin of the Arduino.

Connect the data pins of the 16x2 LCD Module (D4-D7) to pins 6, 5, 4, and 3 of the Arduino. Connect the RS and E pins of the LCD to pins 8 and 7, respectively.

Connect a push button to pin 2 of the Arduino.

Connect an LED to pin 11 of the Arduino.

The circuit design ensures proper connections and communication between the components.

Code
The Arduino code for the Auto Intensity Control of Street Lights is provided in the code section of the project. The code is responsible for reading data from the DS3231 RTC Module, the LDR, and adjusting the LED brightness based on the detected ambient light.

Working
In RTC Mode, the Arduino reads the time from the DS3231 RTC Module. If the current time matches the ON time specified in the code, the street lights are turned on. Similarly, if the current time matches the OFF time, the street lights are turned off.

In LDR Mode, the Arduino reads the LDR values, which represent the ambient light level. The brightness of the LED street lights is adjusted based on the LDR readings. As the ambient light increases or decreases, the LED brightness changes accordingly.

The 16x2 LCD display is used to show the current time and the status of the street lights (ON/OFF) in RTC Mode, or the brightness level in LDR Mode.

Usage
Assemble the circuit as per the provided circuit diagram.

Upload the provided Arduino code to the Arduino board.

Power up the circuit and observe the behavior of the street lights based on the selected mode (RTC or LDR).

In RTC Mode, the street lights will automatically turn on and off at the specified times.

In LDR Mode, the street lights' brightness will adjust based on the surrounding light conditions.

The Auto Intensity Control of Street Lights using Arduino project provides an energy-efficient solution for street lighting by dynamically adjusting the light intensity according to the environmental conditions, thereby saving power and promoting sustainability.