# Sensor Datasheets and Info

## 1. FSR (Force Sensitive Resistor) Pressure Sensor

- **Type:** Analog Force/Pressure Sensor  
- **Operating Voltage:** 0-5V (compatible with Arduino/NodeMCU ADC)  
- **Output:** Variable resistance changes with pressure (read via analog input)  
- **Range:** Typically 100g to 10kg  
- **Pinout:**  
  - Two terminals: connect one to voltage (3.3V or 5V) and the other to analog input with pull-down resistor  
- **Description:**  
  Detects pressure by changing resistance when force is applied.  
- **Use in LibriSense:**  
  Detects if someone is sitting in a seat to monitor occupancy.  
- **Datasheet Link:**  
  [FSR Datasheet PDF](https://cdn.sparkfun.com/datasheets/Sensors/ForceFlex/FlexibleForceSensor.pdf)

## 2. DHT11 Temperature & Humidity Sensor

- **Type:** Digital Temperature and Humidity Sensor  
- **Operating Voltage:** 3.3V to 5V DC  
- **Output:** Digital signal (single-wire protocol)  
- **Pinout:**  
  - VCC: Power (+3.3V or +5V)  
  - GND: Ground  
  - DATA: Digital output pin  
  - (Sometimes a 4th NC pin)  
- **Description:**  
  Measures ambient temperature and humidity, simple and low cost.  
- **Use in LibriSense:**  
  Monitors environment conditions inside the library.  
- **Datasheet Link:**  
  [DHT11 Datasheet PDF](https://cdn-shop.adafruit.com/datasheets/DHT11.pdf)

## 3. Voice Sound Detection Microphone Module

- **Type:** Analog Sound Detection Module  
- **Operating Voltage:** 3.3V to 5V DC  
- **Output:** Digital output (sound detected or not) and sometimes analog output (sound intensity)  
- **Pinout:**  
  - VCC: Power supply  
  - GND: Ground  
  - DO: Digital output  
  - AO: Analog output (if available)  
- **Description:**  
  Detects presence of sound, triggers digital output when sound exceeds threshold.  
- **Use in LibriSense:**  
  Detects ambient noise or user voice presence for alerts or interactions.  
- **Datasheet Link:**  
  [Generic Sound Sensor Module](https://lastminuteengineers.com/sound-sensor-arduino-tutorial/)

## 4. Ultrasonic Sensor Module (HC-SR04)

- **Type:** Ultrasonic Distance Sensor  
- **Operating Voltage:** 5V DC  
- **Output:** Digital pulse width proportional to distance  
- **Pinout:**  
  - VCC: 5V power  
  - GND: Ground  
  - TRIG: Trigger pin (input)  
  - ECHO: Echo pin (output)  
- **Description:**  
  Measures distance by sending ultrasonic pulses and measuring echo time.  
- **Use in LibriSense:**  
  Detects proximity or presence near bookshelves or seats.  
- **Datasheet Link:**  
  [HC-SR04 Datasheet PDF](https://components101.com/sites/default/files/component_datasheet/HC-SR04%20Datasheet.pdf)

## 5. RFID Tag and Reader (MFRC522)

- **Type:** RFID Reader Module  
- **Operating Voltage:** 3.3V DC  
- **Output:** SPI communication interface  
- **Pinout:**  
  - VCC: 3.3V power supply  
  - GND: Ground  
  - RST: Reset pin  
  - IRQ: Interrupt (optional)  
  - MISO, MOSI, SCK, SDA: SPI pins  
- **Description:**  
  Reads RFID tags to identify books or users.  
- **Use in LibriSense:**  
  For book or user identification via RFID tags.  
- **Datasheet Link:**  
  [MFRC522 Datasheet PDF](https://www.nxp.com/docs/en/data-sheet/MFRC522.pdf)

## 6. NodeMCU ESP8266 Module

- **Type:** WiFi Development Board based on ESP8266  
- **Operating Voltage:** 3.3V DC  
- **Features:**  
  - Integrated WiFi for IoT connectivity  
  - GPIO pins for sensor interfacing  
  - Supports Arduino IDE programming  
- **Use in LibriSense:**  
  Acts as the main microcontroller handling sensors and sending data to the cloud/server.  
- **Datasheet Link:**  
  [NodeMCU ESP8266](https://nodemcu.readthedocs.io/en/release/)

