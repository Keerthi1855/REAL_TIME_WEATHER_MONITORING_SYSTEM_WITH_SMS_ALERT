# REAL_TIME_WEATHER_MONITORING_SYSTEM_WITH_SMS_ALERT

## Project Overview

This project is a **Real-Time Weather Monitoring and GSM Alert System** developed using the **ARM7 LPC2129 microcontroller**. The system continuously monitors the ambient temperature using an **LM35 temperature sensor**, displays the current temperature along with real-time clock information on a **16×2 LCD**, and automatically sends an SMS alert through a **GSM module** whenever the temperature exceeds a predefined threshold (28°C).

The project demonstrates the implementation of multiple communication protocols, including **SPI**, **I2C** and **UART** making it a practical embedded systems application for environmental monitoring and remote alerting.


## Features

* 🌡️ Real-time temperature monitoring using the **LM35** sensor.
* 🕒 Displays current time using an **RTC (DS1307)**.
* 📟 16×2 LCD displays:

  * Current Time
  * Temperature
* 📩 Sends automatic SMS alerts using a GSM module when the temperature exceeds **28°C**.
* 🔄 Continuous real-time monitoring.
* ⚡ Demonstrates hardware interfacing using SPI, I2C, and UART communication protocols.


## Hardware Components

* ARM7 LPC2129 Microcontroller
* LM35 Temperature Sensor
* MCP3204 SPI ADC
* DS1307 RTC Module
* GSM Module (SIM800/SIM900)
* 16×2 LCD Display
* Power Supply


## Software & Tools

* Embedded C
* Keil μVision
* Flash Magic


## Communication Protocols

| Peripheral  | Protocol |
| ----------- | -------- |
| MCP3204 ADC | SPI      |
| DS1307 RTC  | I2C      |
| GSM Module  | UART     |


## Working Principle

1. The LM35 senses the surrounding temperature.
2. The MCP3204 ADC converts the analog output of the LM35 into digital data using the SPI protocol.
3. The LPC2129 reads the temperature and displays it on the LCD.
4. The RTC provides the current time through the I2C protocol.
5. If the temperature exceeds **28°C**, the LPC2129 communicates with the GSM module through UART and sends an SMS alert to the predefined mobile number.
6. The system continuously updates the temperature and time in real time.


## Technologies Used

* Embedded C
* ARM7 LPC2129
* SPI Communication
* I2C Communication
* UART Communication
* ADC Interfacing
* GSM Communication
* Real-Time Clock (RTC)

## Applications

* Weather Monitoring Systems
* Industrial Temperature Monitoring
* Greenhouses
* Server Rooms
* Laboratories
* Cold Storage Monitoring

## Future Enhancements

* Add humidity sensing using DHT11/DHT22.
* Store temperature logs on an SD card.
* Upload sensor data to a cloud platform.
* Implement configurable temperature thresholds.
* Develop a mobile application for remote monitoring.


## Author

**Keerthana A**


