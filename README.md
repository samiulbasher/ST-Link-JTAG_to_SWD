# ST-Link JTAG to SWD Adapter

A simple, compact adapter that converts a legacy ARM 20-pin JTAG/SWD IDC connector to a standard SWD header. Compatible with ST-Link, J-Link, and other JTAG-based programmers.

---

## 🧰 General

This adapter is designed for developers to **simplify the development and debugging process**.

Instead of dealing with messy jumper wires or complex breakout boards, this provides a clean and reliable solution for converting JTAG to SWD—ideal for use with:

- ST-Link  
- J-Link  
- Other generic JTAG programmers

---

## 📌 Features

- **Plug & Play** — No need to look up datasheets or pinouts  
- **Developer-Friendly** — Saves time and reduces frustration  
- **Labeled Pins** — Clear labeling right on the PCB  
- **Reduces Errors** — Focus on your work, not wiring  
- **Compact** — Just 30x31 mm in size (*2-layer PCB*)

---

## 🧾 Applications

- Debugging and programming ARM Cortex-M microcontrollers  
- Quick SWD access for STM32 and other ARM-based chips  
- Works with any 20-pin JTAG header programmer

---

## 📷 Board Images

> Photos of the adapter and panelized PCB:

![ST-Link V2 JTAG to SWD Adapter](https://github.com/user-attachments/assets/4ddc6696-c4ac-4d62-91f4-aacd9e46ecbd)  
![ST-Link V3 JTAG to SWD Adapter](https://github.com/user-attachments/assets/28d0defd-ff10-4b3d-8655-53fbd2b5a660)  
![Panelized Board](https://github.com/user-attachments/assets/1c1da1a3-f347-49c1-b40f-b52d05483847)
![JTAG to SWD Adapter](https://github.com/user-attachments/assets/614cca4d-5dbb-46a6-8a9f-24a79b867c5d)


---

## 📍 Pin Details

All pin names are printed directly on the PCB.  
Here's a reference for the minimum required connections:

- **4 Pins** (1, 2, 3, 4) — Programming only  
- **6 Pins** (1, 2, 3, 4, 5, 6) — Full debugging + programming

---

## 🔌 Jumper Connection

When using different ST-Link versions:

- **Genuine ST-Link V2 or V3**:  
  Connect `VTarget (VTr)` to the target board's `VDD`.

- **Clone ST-Link usally ST-Link V2 (e.g., Chinese versions)**:  
  Connect the adapter's **3.3V** pin to the target's `VDD`.

---

## 📦 Specifications

| Attribute           | Value                            |
|---------------------|----------------------------------|
| Dimensions           | 30 mm x 31 mm                   |
| Connector Type       | ARM 20-pin JTAG to SWD Header   |
| Programmer Support   | ST-Link, J-Link, and others     |

---

## ✅ Compatibility

| Programmer       | Compatible |
|------------------|------------|
| ST-Link V2       | ✅         |
| ST-Link V3       | ✅         |
| J-Link           | ✅         |
| Other JTAG headers | ✅       |

---



---

## 📁 Design Files & Gerber Files

- The `JTAG_to_SWD/` directory contains the original **KiCad project files**.  
  If you’d like to modify or customize the board, you can easily do so using KiCad.

- The `gerber/` directory includes **production-ready files** for PCB manufacturing.

  Inside it, you’ll find a `panel/V1.1/` subfolder — this contains the **panelized version** of the PCB (`JTAG_to_SWD_panel_V1.1.zip`).  
  This file is ready to upload directly to [JLCPCB](https://jlcpcb.com) for manufacturing.

💡 This is a **2-layer PCB**, and each panel contains **6 individual boards**.  
That means for just **$2**, you can get **30 PCBs** produced at JLCPCB!

---

## 📝 License

This project is released under the [MIT License](LICENSE).

