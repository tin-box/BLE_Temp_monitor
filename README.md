# BLE_Temp_monitor
Arduino Temperature monitor that uses BLE to share data
# WiFi Mesh Temperature Monitor
## Introduction

I wrote this to make an array of low cost, low power temperature sensors that can cover a large area by linking together through a WiFi Mesh approach.  Nodes connect to nodes with the strongest signal and relay data through the mesh so that each node has the temp and humidity data of all other nodes.  If a temperature exceeds a configured limit a buzzer in that Node as well as the Buzzer in Node 0 will sound.

I worked this until I had a working version and then iterated a few versions fixing obvious bugs and then shelved it.  Feel free to build on what I have done and extend it for other purposes.  Have Fun!
## Software/Firmware 
See the Setup section below for instructions to get his running. I have built it with both Arduino package as well as VS Code successfully.  To configure WiFi access password Node number and related item make changes in the Config.h file.

# Setup
Getting started with ESP-IDF on IDE Arduino

1.      Install Arduino IDE

Download and install the Arduino IDE for your PC platform

[https://www.arduino.cc/en/software](https://www.arduino.cc/en/software)

2.      Configure Arduino preferences with Espressif IDE package

![](file:///C:/Users/mattt/AppData/Local/Temp/msohtmlclip1/01/clip_image001.png)

In the “Additional Boards Manager URLs:” box enter [https://dl.espressif.com/dl/package_esp32_index.json](https://dl.espressif.com/dl/package_esp32_index.json)

![](file:///C:/Users/mattt/AppData/Local/Temp/msohtmlclip1/01/clip_image002.png)![](file:///C:/Users/mattt/AppData/Local/Temp/msohtmlclip1/01/clip_image004.jpg)

3.      Install ESP32 in Arduino Manager

![](file:///C:/Users/mattt/AppData/Local/Temp/msohtmlclip1/01/clip_image005.png)![](file:///C:/Users/mattt/AppData/Local/Temp/msohtmlclip1/01/clip_image006.png)

Search for ESP32

Select install

![](file:///C:/Users/mattt/AppData/Local/Temp/msohtmlclip1/01/clip_image007.png)![](file:///C:/Users/mattt/AppData/Local/Temp/msohtmlclip1/01/clip_image008.png)![Graphical user interface, text, application, email
Description automatically generated](file:///C:/Users/mattt/AppData/Local/Temp/msohtmlclip1/01/clip_image010.jpg)

4.      Install Libraries in Arduino library tree

![](file:///C:/Users/mattt/AppData/Local/Temp/msohtmlclip1/01/clip_image011.png)![A screenshot of a computer
Description automatically generated with medium confidence](file:///C:/Users/mattt/AppData/Local/Temp/msohtmlclip1/01/clip_image013.jpg)

5.      Open Temp sensor source code

Edit Config.h file SENSOR_NUMBER  such that Main node = 0, Sensor1 = 1, Sensor2 = 2 etc.

![](file:///C:/Users/mattt/AppData/Local/Temp/msohtmlclip1/01/clip_image014.png)![Text
Description automatically generated with medium confidence](file:///C:/Users/mattt/AppData/Local/Temp/msohtmlclip1/01/clip_image016.png)

  

6.      Select ESP32 board COM port

![](file:///C:/Users/mattt/AppData/Local/Temp/msohtmlclip1/01/clip_image008.png)![](file:///C:/Users/mattt/AppData/Local/Temp/msohtmlclip1/01/clip_image018.jpg)

7.      Compile and Flash software onto ESP32 board

![](file:///C:/Users/mattt/AppData/Local/Temp/msohtmlclip1/01/clip_image019.png)![](file:///C:/Users/mattt/AppData/Local/Temp/msohtmlclip1/01/clip_image020.png)


## Bill of Materials

| Part No | Description | Qty |
|---|---|---|
|esp32-1.14lcdttgo-001|1.14 Inch LCD ESP32 WiFi And Bluetooth Module|7|
|aht10-i2c-001|AHT10 Digital Temperature Sensor Module I2C|7|
|90db_dc3-24v-001|Active Piezo Buzzer 90 db 2-Wire DC 3-24V|7|
|usb6ft-001|USB Type-C Cable 6ft type C to A Cable braided - grey|7|
|pwr1a5v-001|USB Charger Adapter 1A/5V Single Port - black|7|
|nylon-2mm-5.6mm-001|Push Clip Rivet 2mm x 5.6mm PCB Circuit Panel Nylon Fastener - Black|28|
|esp32tdbtm-001|ESP32 TDisplay Bottom|7|
|esp32tdtop-001|ESP32 TDisplay Top_Tall|7|
