# 🐓 Poultry Floor Cleaning & Water Spraying System

An Arduino-based automation project for poultry farms that remotely controls floor cleaning and water spraying, and also alerts when the manure bin is full using an ultrasonic sensor and buzzer.

## 🚀 Features

- IR Remote controlled:
  - Toggle floor movement (relay)
  - Toggle water spraying (relay)
  - Combo mode (floor + pump together)
- Manure bin fullness detection with ultrasonic sensor
- Audible alert with buzzer when bin is full

## 🧰 Components Used

- Arduino Uno
- IR Remote & Receiver (TSOP1738 or similar)
- Ultrasonic Sensor (HC-SR04)
- 2-Channel Relay Module
- Buzzer
- Wires, Breadboard, Power supply

## 🖥️ Pin Configuration

| Component           | Arduino Pin |
|---------------------|-------------|
| Floor Motor Relay   | D4          |
| Water Pump Relay    | D5          |
| IR Receiver         | D7          |
| Ultrasonic Trigger  | D9          |
| Ultrasonic Echo     | D8          |
| Buzzer              | D11         |

> ⚠️ Relays are Active LOW (LOW = ON, HIGH = OFF)

## 📦 IR Remote Codes

Replace with your actual remote’s hex codes:

| Function         | Hex Code     |
|------------------|--------------|
| Floor ON         | 0x1FEC13E    |
| Floor OFF        | 0x1FEE41B    |
| Pump ON          | 0x1FEE11E    |
| Pump OFF         | 0x1FE916E    |
| Combo ON         | 0x1FE12ED    |
| Combo OFF        | 0x1FE817E    |

Use the `IRrecvDumpV2` example in the IRremote library to get your codes.

## 📷 Future Upgrades

- Servo to dispense feed
- Stepper to rotate medicine sprayer
- Bluetooth or Wi-Fi remote control
- LCD for system status

## 📝 License

MIT License — feel free to use and modify!
# poultry-cleaning-system
