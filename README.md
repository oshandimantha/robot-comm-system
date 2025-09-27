# 🚗 LoRa Joystick Controlled Robot Car

This project is a robot car built using **2 hoverboard motors**, **ZS-X11H motor controllers**, and **Arduino Nano** boards with **LoRa communication**.  
The system uses a joystick for wireless control, supporting smooth forward, reverse, and turning movements.

---

## 📂 Repository Structure
```
/receiver     → Arduino Nano code for motor driver (with ramping, deadzone, debug prints)
/transmitter  → Arduino Nano code for joystick input and LoRa transmission
/docs         → Circuit diagrams, images, wiring screenshots
```

---

## 🔧 Hardware Used
- 2 × Hoverboard motors
- 2 × ZS-X11H controllers
- 2 × Arduino Nano
- 2 × LoRa SX1278 modules
- Joystick module
- Power supply (24V battery)

---

## ⚡ Features
- Smooth PWM ramping (no sudden jerks)
- Adjustable **deadzone**, **max speed**, and **invert motor logic**
- Serial debug prints for troubleshooting
- Forward, Reverse, Left, Right movement
- LoRa communication (433 MHz)

---

## 📜 How to Use
1. Upload `transmitter/transmitter.ino` to the **joystick Nano**.
2. Upload `receiver/receiver.ino` to the **motor Nano**.
3. Connect motors & controllers as per wiring diagram in `/docs`.
4. Power both Arduinos and enjoy wireless driving!

---

## 🛠️ User Adjustable Settings
In the receiver code (top section), you can easily tune:
- `DEADZONE` → Ignore joystick noise
- `MAX_PWM_FORWARD` / `MAX_PWM_REVERSE` / `MAX_PWM_TURN`
- `INVERT_LEFT` / `INVERT_RIGHT`

---

## 📄 License
MIT License
