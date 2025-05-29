# HuskyLens Face Recognition Door Lock with Arduino

This project uses the **HuskyLens AI Camera** for face recognition to control a door lock system using an **Arduino board**. When a known face is detected, the lock is automatically released via a relay module.

## 🧰 Requirements

Before you begin, ensure you have the following components:

- 🔐 **Electronic Door Lock** (e.g., solenoid or magnetic lock)
- ⚡ **Relay Module** (to control the lock)
- 📷 **HuskyLens AI Camera**
- 💻 **Arduino Board** (e.g., Uno, Nano, Mega)
- 🚪 **Door** (for physical installation)
- 🔌 Power supply (5V or 12V depending on your lock)

Optional:
- Jumper wires
- Breadboard or mounting hardware
- Enclosure for electronics

## ⚙️ Wiring Overview

1. **HuskyLens → Arduino**
   - TX → RX (pin 0)
   - RX → TX (pin 1)
   - GND → GND
   - VCC → 5V

2. **Relay Module → Arduino**
   - IN → Digital pin (e.g., D7)
   - VCC → 5V
   - GND → GND

3. **Lock → Relay**
   - Connect power supply and lock through relay as per your lock’s specifications.

> ⚠️ **Important:** Ensure proper power ratings for the lock and protect the circuit against overcurrent if needed.

## 🔄 How It Works

1. HuskyLens is trained to recognize one or more faces.
2. It continuously scans for recognized faces.
3. When a trained face is detected, Arduino triggers the relay.
4. The relay activates the electronic lock to open the door.

## 🚀 Getting Started

1. **Train HuskyLens:**
   - Use the onboard screen and buttons to train your face using "Face Recognition" mode.
   - Save the ID (e.g., ID1 for the primary user).

2. **Upload Arduino Code:**
   - Use the Arduino IDE to upload the provided `.ino` sketch.
   - The code listens to HuskyLens data and controls the relay.

3. **Power up and Test:**
   - Connect all components.
   - Power the system.
   - Approach the HuskyLens with a trained face—watch the door unlock!

## 📂 File Structure


