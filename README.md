# Smart Helmet and Vehicle Safety System

This project is an Arduino-based smart helmet safety system designed to improve rider safety.

The system checks:

- Helmet wearing status using IR sensor
- Alcohol detection using MQ2 sensor

The helmet unit sends data wirelessly using RF Transmitter and Receiver modules.

The vehicle starts only when:
- Helmet is worn
- No alcohol is detected

## Features

- Wireless communication using 433MHz RF module
- Alcohol detection
- Helmet detection
- Vehicle ignition control using relay
- LCD status display
- Safety indication LEDs
- Push button ignition system

## Components Used

### Helmet Unit
- Arduino UNO
- IR Sensor
- MQ2 Alcohol Sensor
- RF Transmitter
- LEDs
- Breadboard
- Jumper Wires

### Vehicle Unit
- Arduino UNO
- RF Receiver
- Relay Module
- LCD I2C Display
- Push Button
- LEDs
- Breadboard

## Working Principle

1. IR sensor checks whether the rider is wearing the helmet.
2. MQ2 sensor detects alcohol level.
3. Helmet Arduino sends:
   - SAFE
   - HELMET_OFF
   - ALCOHOL
4. Vehicle Arduino receives the message.
5. Relay allows vehicle ignition only when safe conditions are satisfied.

## Libraries Used

- RH_ASK
- SPI
- Wire
- LiquidCrystal_I2C

## Future Improvements
- Bluetooth/WiFi communication
- GPS tracking
- GSM emergency alert
- Accident detection
- Mobile App integration

## Authors
- Gagan A
- Bharath N S
- Aditya R Khot
- Bhavana R
