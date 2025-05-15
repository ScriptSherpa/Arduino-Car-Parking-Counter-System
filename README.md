


# 🚗 Arduino Car Parking Counter System

An Arduino-based Smart Car Parking Counter System that uses an ultrasonic sensor, LCD display, and servo motor to detect and count cars entering and exiting a parking lot. This system displays the total number of cars currently parked in the lot on an LCD screen.

---

## 📷 Project Preview

<img src="https://github.com/ScriptSherpa/Arduino-Car-Parking-Counter-System/blob/bf893064fdac799ac31dd4d16dda2cf69ffbb5de/media/WhatsApp%20Image%202025-05-14%20at%2019.44.58.jpeg?raw=true" alt="Arduino Parking System" width="600"/>
  
*Image: Working prototype with LCD and Ultrasonic Sensor*

---

## 🛠️ Hardware Components

| Component              | Quantity |
|------------------------|----------|
| Arduino Uno            | 1        |
| Ultrasonic Sensor (HC-SR04) | 1        |
| 16x2 LCD Display (I2C) | 1        |
| Servo Motor (SG90)     | 1        |
| Breadboard & Wires     | As needed |
| Power Supply (5V/USB)  | 1        |

---

## 🔌 Circuit Diagram

> Replace the link below with your actual image hosted on Imgur or another image service.
<img src="## 🔌 Circuit Diagram

<img src="https://github.com/ScriptSherpa/Arduino-Car-Parking-Counter-System/blob/d41d3b6c6d79b4b625a1bc1fb637d32fb2897275/Automatic-Visitor-Counter/automatic-visitor-counter-circuit.jpg?raw=true" alt="Automatic Visitor Counter Circuit" width="600"/>



## 📄 How It Works

- The **ultrasonic sensor** detects an approaching car.
- The **servo motor** simulates a gate barrier, which lifts when a car passes.
- The system **counts cars entering and exiting** the parking area.
- The **16x2 LCD display** shows the current number of cars inside the parking lot.
- You can enhance this system by using **two ultrasonic sensors** to differentiate entry and exit lanes.

---

## 🧠 Logic

- If distance < threshold (e.g., 10 cm), it means a car is detected.
- The servo opens the gate for a short duration.
- The count is increased or decreased based on direction (optional feature with dual sensors).
- The LCD updates with the new count.

---

## 🖥️ Sample Output (LCD Display)

```

Cars In: 5
Cars Out: 3
In Parking: 2

```

---

## 📦 Arduino Libraries Used

- `LiquidCrystal_I2C.h` – for I2C LCD display
- `Servo.h` – for controlling the servo motor

Install them from the Arduino Library Manager if not already installed.

---

## 🚀 Getting Started

### 1. Wiring

- Connect the **HC-SR04**:  
  - VCC → 5V  
  - GND → GND  
  - TRIG → Digital Pin 9  
  - ECHO → Digital Pin 10

- Connect the **Servo Motor**:  
  - Signal → Digital Pin 6  
  - VCC → 5V  
  - GND → GND

- Connect the **LCD (I2C)**:  
  - SDA → A4  
  - SCL → A5  
  - VCC → 5V  
  - GND → GND

### 2. Upload Code

Use Arduino IDE and upload the code to your Uno board.

---

## 📁 Project Structure

```

📦 Car-Parking-Counter
┣ 📜 README.md
┣ 📜 parking\_counter.ino
┣ 📷 images/
┃ ┗ project\_photo.jpg
┃ ┗ circuit\_diagram.png

```

---

## ✨ Features

- Real-time car counting using distance detection
- Automatic gate opening with a servo
- LCD display of in/out/parked cars
- Expandable for RFID or GSM integration

---

## 💡 Future Enhancements

- Add IR sensors for more accurate entry/exit detection
- Use a buzzer or LED indicator for parking full status
- Integrate with IoT to monitor from a web dashboard

---

## 📜 License

MIT License – feel free to use and modify this project for learning and academic purposes.


---

