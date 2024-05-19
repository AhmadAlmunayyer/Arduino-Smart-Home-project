# Smart Home Model Project

## Introduction
The Smart Home Model Project aims to create a simple and efficient home automation system using Arduino and various sensors. This DIY project allows users to control various functions in their home using an Arduino microcontroller and sensors. The project utilizes RFID, rain sensor, flame sensor, and PIR sensor along with a servo motor, buzzer, and LED to manage different smart home functionalities.

## Features
- **RFID-based door control**
- **Rain sensor-controlled window closing**
- **Flame sensor-triggered fire alarm**
- **PIR sensor-based motion detection for lighting**

## Hardware Requirements
To build this project, you will need the following components:
1. Arduino Uno (1x)
2. RFID-RC522 Module (1x)
3. Servo Motor (2x)
4. Rain Sensor Module (1x)
5. Flame Sensor Module (1x)
6. Buzzer (1x)
7. PIR Motion Sensor (1x)
8. LED (1x)
9. Breadboard (1x)
10. Jumper wires (assorted)
11. Resistor (220 Ohm) (1x)
12. Power supply (5V)

## Software Requirements
1. Arduino IDE (latest version)
2. MFRC522 Library for the RFID module

## Circuit Design
Follow these steps to set up the circuit:
1. **Connect the Arduino Uno to the breadboard.**
2. **Connect the RFID-RC522 module to the Arduino:**
   - SDA to pin 10
   - SCK to pin 13
   - MOSI to pin 11
   - MISO to pin 12
   - GND to GND
   - RST to pin 9
   - 3.3V to 3.3V
3. **Connect the first servo motor (door control) to the Arduino:**
   - Signal pin to pin 3
   - VCC to 5V
   - GND to GND
4. **Connect the rain sensor to the Arduino:**
   - Data pin to A0
   - VCC to 5V
   - GND to GND
5. **Connect the second servo motor (window control) to the Arduino:**
   - Signal pin to pin 5
   - VCC to 5V
   - GND to GND
6. **Connect the flame sensor to the Arduino:**
   - Data pin to A1
   - VCC to 5V
   - GND to GND
7. **Connect the buzzer to the Arduino:**
   - Positive pin to pin 6
   - Negative pin to GND
8. **Connect the PIR motion sensor to the Arduino:**
   - Data pin to pin 2
   - VCC to 5V
   - GND to GND
9. **Connect the LED to the Arduino:**
   - Anode (longer leg) to pin 7 via a 220 Ohm resistor
   - Cathode (shorter leg) to GND

## Code Overview
1. **Import required libraries.**
2. **Declare pins and variables.**
3. **Initialize serial communication, RFID module, and servo motors.**
4. **In the main loop:**
   - Check for RFID tag and validate. If valid, control the door servo motor.
   - Read rain sensor data and control the window servo motor.
   - Read flame sensor data and trigger the buzzer if a fire is detected.
   - Read PIR motion sensor data and control the LED.

## Installation and Setup
1. Install the Arduino IDE on your computer.
2. Install the MFRC522 library using the Library Manager in the Arduino IDE.
3. Connect the Arduino Uno to your computer using a USB cable.
4. Open the Arduino IDE and copy the provided code.
5. Select your board (Arduino Uno) and the correct COM port.
6. Upload the code to the Arduino.

## Testing and Troubleshooting
1. **Test the RFID door control:** Place a valid tag near the RFID module. The door servo motor should respond.
2. **Test the rain sensor:** Simulate rain with a wet cloth or finger. The window servo motor should respond.
3. **Test the flame sensor:** Simulate a fire with a lighter or a candle. The buzzer should sound.
4. **Test the PIR motion sensor:** Move your hand near the sensor. The LED should illuminate.

If any of the features do not work as expected, check the connections, verify the code, and ensure the components are functioning correctly.

## Conclusion
The Smart Home Model Project using Arduino and various sensors demonstrates the limitless possibilities of technology in home automation. The integration of RFID, rain sensor, flame sensor, and PIR sensor showcases the ability to control different aspects of a home, making it more efficient, comfortable, and secure. This project highlights the versatility of Arduino in handling multiple tasks and serves as an excellent example of how technology can enhance our lives.

## Contributors
- Mohammad AlNajjar
- Hasan Barjawi
- Abdallah Abdelhamid
- Ahmad Abu-Diak
- Ahmad ALMunayyer
- Osama Awad
- Mohammad Ali