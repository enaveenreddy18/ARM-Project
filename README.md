# Smart Healthcare Patient Health Monitoring and Emergency Assistance System using LPC2129

An IoT-based patient health monitoring system developed using the **LPC2129 (ARM7)** microcontroller. The project continuously monitors vital health parameters such as **Heart Rate**, **SpO2**, **Body Temperature**, and **Distance**, displays them on an LCD, and transmits the collected data over Wi-Fi for remote monitoring.

---

## Features

- Real-time Heart Rate monitoring
- SpO2 (Blood Oxygen Saturation) measurement using MAX30102
- Body Temperature monitoring using DHT11
- Distance measurement using HC-SR04 Ultrasonic Sensor
- LCD display for local monitoring
- UART communication for debugging and data transmission
- Bluetooth connectivity for monitoring the patient condition time to time
- Warning indication using LED and Buzzer when abnormal conditions are detected

---

## Hardware Components

- LPC2129 (ARM7) Microcontroller
- MAX30102 Pulse Oximeter Sensor
- DHT11 Temperature Sensor
- HC-SR04 Ultrasonic Sensor
- 16x2 LCD
- HC-05 Bluetooth module 
- Buzzer
- Warning LED

---

## Software & Tools

- Embedded C
- Keil uVision
- LPC2129 ARM7
- UART Communication
- I2C Communication
- GPIO Programming
- Timer Programming
- Interrupt Handling

---

## Repository Structure

```
├── main.c              # Main application
├── header.h            # Function declarations and macros
├── delay.c             # Delay routines
├── uart0_driver.c      # UART driver
├── i2c_driver.c        # I2C driver
├── lcd_driver.c        # LCD driver
├── temparature.c       # DHT11 temperature sensor driver
├── saline_level.c      # Ultrasonic sensor driver
├── iot.c               # MAX30102 interface and IoT communication
├── heart.c             # Heart rate algorithm
├── spo2.c              # SpO2 calculation algorithm
├── interrupt.c         # Interrupt handling
├── handler.c           # Exception handlers
└── README.md
```

---

## Getting Started

### Clone the Repository

```bash
git clone https://github.com/<your-username>/patient-health-monitoring-lpc2129.git
```

Move into the project folder

```bash
cd patient-health-monitoring-lpc2129
```

---

## Build

Open the project in **Keil uVision**.

Build the project using:

```
Project → Build Target
```

Flash the generated HEX file to the LPC2129 development board.

---

## Functional Overview

The system continuously performs the following operations:

1. Initializes LCD, UART, I2C, GPIO, and peripherals.
2. Reads temperature from the DHT11 sensor.
3. Collects Red and IR samples from the MAX30102 sensor.
4. Calculates Heart Rate and SpO2 using signal-processing algorithms.
5. Measures distance using the HC-SR04 ultrasonic sensor.
6. Displays sensor readings on the LCD.
7. Sends sensor data through UART/Bluetooth for monitoring.
8. Activates the warning LED and buzzer whenever abnormal conditions are detected.

---

## Communication Interfaces

- UART
- I2C
- GPIO
- Timer
- External Interrupts

---
## Concepts Demonstrated
- Embedded C Programming
- ARM7 (LPC2129)
- Sensor Interfacing
- Driver Development
- UART Communication
- I2C Communication
- Embedded Signal Processing
- Interrupt Handling
- Real-Time Embedded Systems
---
## Future Improvements
- ECG Sensor Integration
- Cloud Database Storage
- Mobile Application Dashboard
- MQTT Communication
- Real-Time Alerts using SMS/Email
- Battery Monitoring
- Patient History Storage
---
## Contributors
- E. Naveen Kumar Reddy (@enaveenredy18)