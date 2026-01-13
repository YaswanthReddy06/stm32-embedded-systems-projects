# STM32 Embedded Systems Projects

A curated collection of **STM32 embedded systems projects** demonstrating hands-on experience with **bare‑metal firmware, peripheral interfacing, and FreeRTOS‑based real‑time systems** using **STM32CubeIDE**.

This repository is structured as a **mono‑repo**, where each folder represents an independent STM32 project focusing on a specific concept or peripheral.

---

## 🔧 Tech Stack

* **MCU**: STM32 (STM32L4 / STM32F4 family)
* **IDE**: STM32CubeIDE (Eclipse‑based)
* **RTOS**: FreeRTOS
* **Drivers**: STM32 HAL, CMSIS
* **Languages**: C
* **Debug**: ST‑LINK

---

## 📂 Repository Structure

```
stm32-embedded-systems-projects/
│
├── Hello_world/
├── Module1_HelloWorld/
├── Module2_GPIO_SOS/
├── Module2_Interrupt_Button/
├── Module3_FreeRTOS_SOSTask/
├── Module4_UART_TX/
├── Module4_UART_RX_Polling/
├── Module4_UART_RX_Interrupt_Queue/
├── Module5_I2C_TempSensor/
├── Module5_I2C_TempSensorDriver/
├── Module6_I2C_TempSensorDriverInterrupt/
└── README.md
```

Each module is a **standalone STM32CubeIDE project** with its own CubeMX configuration (`.ioc`).

---

## 🧪 Project Overview

### 🔹 Hello World

* Basic STM32 project setup
* LED toggle using HAL
* Clock and GPIO initialization

### 🔹 GPIO SOS (Module 2)

* GPIO output control
* SOS pattern implementation using delays
* Bare‑metal timing logic

### 🔹 External Interrupt – Button

* GPIO input interrupt configuration
* EXTI handling
* Debounce logic

### 🔹 FreeRTOS SOS Task (Module 3)

* FreeRTOS kernel integration
* Task creation and scheduling
* SOS pattern implemented as RTOS task
* Demonstrates deterministic timing

### 🔹 UART Communication (Module 4)

* UART TX
* UART RX (Polling)
* UART RX using Interrupt + Queue
* Inter‑task communication via FreeRTOS queues

### 🔹 I2C Temperature Sensor (Module 5 & 6)

* I2C peripheral configuration
* Sensor register read/write
* Driver abstraction layer
* Interrupt‑driven I2C communication

---

## 🧠 Key Concepts Demonstrated

* Bare‑metal vs RTOS firmware design
* Task scheduling and prioritization
* Interrupt handling
* Peripheral driver development
* Queue‑based inter‑task communication
* Modular firmware architecture

---

## 🏗️ Build Instructions

1. Clone the repository

```bash
git clone https://github.com/<your-username>/stm32-embedded-systems-projects.git
```

2. Open **STM32CubeIDE**
3. Import project:

   * `File → Import → Existing Projects into Workspace`
   * Select the desired module folder
4. Build and flash using **ST‑LINK**

> ⚠️ Note: Generated build files (`Debug/`, `.elf`, `.map`, etc.) are intentionally ignored via `.gitignore`.

---

## 📌 Design Choices

* HAL drivers are committed for reproducibility
* CubeMX `.ioc` files are version‑controlled
* Build artifacts are excluded for clean version control
* Each module is isolated for clarity and scalability

---

## 🎯 Intended Audience

* Embedded Systems Engineers
* Firmware Developers
* Students learning STM32 & FreeRTOS
* Recruiters reviewing embedded portfolios

---

## 🚀 Future Enhancements

* DMA‑based UART and I2C
* Software timers
* Event groups and semaphores
* Power management modes
* Unit testing for drivers

---

## 👤 Author

**Yaswanth Kodimudi**
Master’s in Computer & Systems Engineering
Focus: Embedded Systems | VLSI | FPGA | RTOS

---

## 📄 License

This repository is intended for educational and portfolio purposes.

---

⭐ *If you find this repository useful, feel free to star it!*
