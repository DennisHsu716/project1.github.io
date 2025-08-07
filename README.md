# Aquarium Automation System
## Summary 
Using Arduino, design an automated aquarium system that enables microcontroller-based temperature monitoring and regulation, ensuring the maintenance of the ideal water temperature in real-time. The core of the system consists of a water temperature sensor, such as the DS18B20, which continuously monitors the water temperature and transmits the data to the Arduino. When the temperature falls below a predetermined threshold, the system activates a heater to raise the water temperature. Conversely, if the temperature exceeds the desired level, the system employs a fan or other cooling devices to lower the temperature.
The entire system is designed for automatic control and can be implemented with a simple circuit. This design creates a stable aquatic environment, making it suitable for breeding tropical fish and other aquatic organisms that require consistent water temperatures. Furthermore, the integration of LED indicators for alarm functions enhances the automation and intelligence of the aquarium.
## Environment
![image](https://github.com/DennisHsu716/project1.github.io/blob/main/image/1.png)
I used two vibration motor mean fan and 16mm MCH Ceramic Heater

## Usage
The water too cold, so the light turn to blue light.

![image](https://github.com/DennisHsu716/project1.github.io/blob/main/image/gif/warm.gif)

Because the MCH let the water back to the set value, so the light back to the green.

![image](https://github.com/DennisHsu716/project1.github.io/blob/main/image/gif/blue%20to%20green.gif)

The water to hot than setting value, so the light turn to red, also the fan start work.

![image](https://github.com/DennisHsu716/project1.github.io/blob/main/image/gif/fan%20work.gif)


The water back to setting value, the light turn to green.

![image](https://github.com/DennisHsu716/project1.github.io/blob/main/image/gif/red%20to%20green.gif)
## About future plans
Replace the cooling and refrigeration devices with more advanced models, and design a base that can conceal the circuit board and battery, thereby enhancing the aesthetic appeal.


# 🐠 Aquarium Automation System

An Arduino-based intelligent aquarium system for real-time temperature monitoring and automatic regulation, designed to maintain a stable aquatic environment for tropical fish and other aquatic life.

---

## 📌 Summary

This project uses an **Arduino microcontroller** to create an automated system capable of:
- Monitoring water temperature in real-time using the **DS18B20** sensor
- Activating a **ceramic heater** when the water is too cold
- Turning on **cooling fans (vibration motors)** when the water is too hot
- Using **LED color indicators** (blue, green, red) to display current system status

The design is fully automatic and easy to implement with a simple circuit. It ensures stable water temperatures, making it ideal for fish breeding environments.

---

## 🧰 Hardware Environment

| Component               | Description                                   |
|------------------------|------------------------------------------------|
| Arduino UNO/Nano       | Main controller                                |
| DS18B20                | Water temperature sensor                       |
| 16mm MCH Heater        | Micro ceramic heater (heating unit)            |
| 2x Vibration Motors    | Used as cooling fans                           |
| LED indicators (RGB)   | Blue (too cold), Red (too hot), Green (normal) |
| Breadboard & wires     | For circuit connection                         |
| Power source           | Battery or USB                                 |

---

## ⚙️ How It Works

- **Too cold:** Temperature below threshold → **Blue LED** turns on, **Heater** activates
- **Back to normal:** Temperature rises to desired value → **Green LED**
- **Too hot:** Temperature above threshold → **Red LED** + **Fan (vibration motor)** activates
- **Back to normal:** Temperature drops → **Green LED**

---

## 🖼️ Images (Usage Demonstration)

| Situation                         | Visual                                                                                               |
|----------------------------------|-------------------------------------------------------------------------------------------------------|
| Too Cold – Blue LED              | ![image](https://github.com/DennisHsu716/project1.github.io/blob/main/image/gif/warm.gif)             |
| Temperature Normal – Green LED   | ![image](https://github.com/DennisHsu716/project1.github.io/blob/main/image/gif/blue%20to%20green.gif)|
| Too Hot – Red LED + Fan Active   | ![image](https://github.com/DennisHsu716/project1.github.io/blob/main/image/gif/fan%20work.gif)       |
| Back to Normal – Green LED       | ![image](https://github.com/DennisHsu716/project1.github.io/blob/main/image/gif/red%20to%20green.gif) |

---

## 🔌 Wiring Diagram

> 📁 **[View Full Wiring Diagram](images/wiring_diagram.png)**
 ![image](https://github.com/DennisHsu716/project1.github.io/blob/main/image/1.png)




