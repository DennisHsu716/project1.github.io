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

> 📁 **[View Full Wiring Diagram]**
 ![image](https://github.com/DennisHsu716/project1.github.io/blob/main/image/1.png)   

[Arduino]  
├── DS18B20 sensor → Digital pin  
├── MCH heater → Transistor/MOSFET switch (powered externally)  
├── Vibration fan → Transistor controlled  
└── RGB LED → 3 digital pins (R, G, B)  

---

## 📈 Future Improvements
* Replace current heater and fan with more efficient, compact components  
* Build a **custom acrylic or 3D-printed base** to hide the battery and circuit board for improved aesthetics  
* Add an LCD display for real-time temperature output  
* Implement mobile app or Bluetooth control

---

## 📁 Folder Structure
Aquarium-Automation/
├── images/
│ ├── blue_light.jpg
│ ├── green_light.jpg
│ ├── red_light.jpg
│ ├── wiring_diagram.png
│ └── ...
├── Arduino_code.ino
└──  README.md


