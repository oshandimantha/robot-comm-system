# RF-Based Robot Communication System (Arduino Nano + 433 MHz)

This project demonstrates a **robot communication system** designed using an **RF module (433 MHz TX/RX)** and two **Arduino Nano** boards.  
It controls actuators (represented by **LEDs**) remotely using a simple communication protocol.

---

## 📌 Part 2: Design a Robot Communication System

### ✅ Chosen Communication Method
- **RF Communication (433 MHz)**  
- Range: A few hundred meters in open environments  
- Low power consumption (12V supply)  
- Low-cost and simple implementation  
- Works reliably indoors and outdoors  

---

## 📐 Step 1: System Requirements
- **Range:** Up to a few hundred meters (depending on obstacles).  
- **Data Rate:** Sufficient for control signals and actuator commands.  
- **Power Consumption:** Minimal to extend battery life.  
- **Environment:** Indoor/outdoor operation with possible interference.  
- **Cost & Complexity:** Low-cost, less complex.  

---

## 📡 Step 2: RF Module
- **433 MHz Transmitter/Receiver pair**  
- Provides a simple and low-cost solution for robot control.  

---

## ⚙️ Step 3: System Design Components
- **Arduino Nano (x2):** One for transmission, one for reception.  
- **RF Transmitter & Receiver:** Handles wireless communication.  
- **LEDs (4 Actuators):** Represent pneumatic actuators.  
- **Power Supply:** 12V external supply / USB.  
- **Serial Monitor:** Debugging and command monitoring.  

---

## 🔄 Step 4: Communication Protocol
- Defined set of single-character commands:  

| Command | Action                  |
|---------|--------------------------|
| `R`     | Turn ON Red LED (Actuator 1) |
| `Y`     | Turn ON Yellow LED (Actuator 2) |
| `B`     | Turn ON Blue LED (Actuator 3) |
| `G`     | Turn ON Green LED (Actuator 4) |
| `S`     | Turn OFF all actuators (Stop) |

---

## 💻 Step 5: Software Implementation
- Arduino IDE used for coding.  
- Libraries:  
  - **RadioHead RH_ASK** (for RF communication).  

---

## 🧪 Step 6: Testing & Debugging
- **Range Testing:** Verified in open area and indoor conditions.  
- **Functional Testing:** Commands tested on Serial Monitor → LEDs respond accordingly.  
- **Debugging:** Serial monitor outputs confirm TX/RX communication.  

---

## ⚡ Step 7: Optimization
- Designed for **one-way communication** (control → actuators).  
- Low power operation to conserve battery.  
- Could be extended with feedback and error-checking.  

---

## 📊 Block Diagram
