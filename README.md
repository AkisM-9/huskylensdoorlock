
HuskyLens Face Recognition Door Lock with Arduino
This project uses the HuskyLens AI Camera for face recognition to control a door lock system using an Arduino board. When a known face is detected, the lock is automatically released via a relay module.

🧰 Requirements
Ensure you have the following components:

🔐 Electronic Door Lock (e.g., solenoid or magnetic lock)

⚡ Relay Module

📷 HuskyLens AI Camera

💻 Arduino Board (e.g., Uno, Nano, Mega)

🚪 Door for mounting

🔌 Power supply (5V or 12V depending on your lock)

Optional:

Jumper wires

Breadboard or mounting hardware

Weatherproof enclosure

⚙️ Wiring Overview
HuskyLens → Arduino (I2C mode)

SDA → A4 (on Uno)

SCL → A5 (on Uno)

GND → GND

VCC → 5V

Relay Module → Arduino

IN → Digital pin 3

VCC → 5V

GND → GND

Lock → Relay

Connect power and lock through relay as per your lock’s datasheet.

⚠️ Make sure to match the lock voltage with the power supply and protect the circuit against surges or overcurrent if needed.

🔄 How It Works
HuskyLens is trained to recognize one or more faces.

Arduino checks if HuskyLens detects a known face.

If a match is found, the relay triggers and unlocks the door.

After 5 seconds, the system relocks automatically.


