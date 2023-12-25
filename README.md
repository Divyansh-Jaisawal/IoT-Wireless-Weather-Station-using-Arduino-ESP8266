# IoT-Wireless-Weather-Station-using-Arduino-ESP8266

Global warming has led to unpredictable climates, prompting researchers to use weather stations to study climate changes and provide forecasts. These stations typically consist of sensors and a monitoring system. This tutorial demonstrates how to build a wireless IoT-based weather station that can measure critical environmental parameters like temperature, humidity, and pressure. The data can be sent to an IoT cloud for remote storage, analysis, and access. Similar weather stations have been built using Raspberry Pi before.

We will be using the Arduino board along with the DHT11 sensor, BMP180 sensor, and an ESP8266 wifi module. The DHT11 sensor senses the temperature and humidity, while the BMP180 sensor calculates the pressure, and ESP8266 is used for internet connectivity. In our previous project, we already learned to use the DHT11 sensor to monitor temperature and humidity with Arduino, here in this project, we are adding another sensor (BMP180) to make a complete weather station using Arduino. Sending these data to ThingSpeak enables live monitoring from anywhere in the world and we can also view the logged data which will be stored on their website and even graph it over time to analyze it.

# Components Required
Arduino Uno
ESP8266 Wi-Fi Shield
DHT11 Sensor
BMP180 Sensor
Breadboard
Jumper Wires

The DHT11 sensor is powered by the 5V pin of the Arduino and its data pin is connected to pin 5 for one-wire communication. The BMP180 sensor is powered by the 3.3V pin of Arduino and its data pins SCL (Serial Clock) and SDA (Serial Data) are connected to the A4 and A5 pin of Arduino for I2C communication.

The ESP8266 module is also powered by the 3.3V pin of the Arduino and its Tx and Rx pins are connected to Digital pins 2 and 3 of Arduino for serial communication. You can use the below table as a reference for making your connections.

S.NO.

Pin Name

Arduino Pin

1

ESP8266 VCC

3.3V

2

ESP8266 RST

3.3V

3

ESP8266 CH-PD

3.3V

4

ESP8266 RX

TX

5

ESP8266 TX

RX

6

ESP8266 GND

GND

7

BMP180 VCC

5V

8

BMP180 GND

GND

9

BMP180 SDA

A4

10

BMP180 SCL

A5

11

DHT-11 VCC

5V

12

DHT-11 Data

5

13

DHT-11 GND

GND

