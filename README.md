# Garden care – Sample mart Soil Assessment Tool for beginner home Gardeners

## 1. Overview
This idea comes from my dad, he loves growing vegetables in our small home garden because he enjoys harvesting food that we can actually eat. My mom, on the other hand, prefers planting flowers like our neighbors do. Over time, I learned that different types of soil are better suited for different kinds of plants, which inspired me to explore this idea further.

## Problem statement

Many beginner home gardeners aren’t sure whether their soil is better for vegetables or flowers, and sometimes they don’t even consider these factors. Differences in soil moisture, pH, and temperature make it hard to predict what will grow well. Without guidance, users may plant or flowers that fail, wasting time and effort. A simple, easy to use tool is needed to help gardeners assess their soil and make informed decisions.

## Detail of design
- A compact soil sensor device inserted directly into the soil(backside)
- A separate display device placed on the frontside for easy viewing of results

---

## 2. Sensor Device

The sensor device is responsible for collecting soil condition data. It is designed to be placed directly into the soil near plants or planting areas.

- Microcontroller: ESP32
- Soil Moisture Sensor: datasheet-[Download Soil Sensor Datasheet](datasheets/soil_sensor.pdf)
- Soil ph sensor: https://docs.rakwireless.com/product-categories/wisnode/soil-ph-monitoring/datasheet/ 

**Description**
The ESP32 processes the sensor data and prepares it for transmission. These measurements represent key indicators of whether the soil environment is suitable for vegetables or flowers.

---

## 3. Display device

The display device receives data from the sensor device and presents the information in a simple and understandable format for users.


- Microcontroller: ESP32-WROOM-32
- Display: OLED Display https://www.mouser.com/datasheet/2/1398/Soldered_333099-3395096.pdf?srsltid=AfmBOoqps0u-2X1SBVf25elJZ8unm8vJw4Sn5SoTNT5sZieUPidi07-d 
- LEDs: Red / Green LEDs for status 

**Description**
The display device receives soil condition data from the sensor device.  
The OLED screen shows whether the soil is suitable for planting, and the LEDs provide quick status feedback.

---

## 4. System Communication Diagram
[Overview Sketch](IMG_2E9451848BBA-1.jpeg)

[Overview Sketch](systemflow.jpg)

## Sceenshot-datasheet
[Overview Sketch](Screenshotdatasheet.png)

## Github link
https://github.com/pzhang23-bit/TECHIN514_SpencerZhang_System-Architecture-with-Diagram.git













