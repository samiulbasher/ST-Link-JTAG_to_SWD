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
- **Compact** — Just 30x31 mm in size

---

## 🧾 Applications

- Debugging and programming ARM Cortex-M microcontrollers
- Quick SWD access for STM32 and other ARM-based chips
- Works with any 20-pin JTAG header programmer

---

## 📷 Board Image

> Add an image of your adapter here  
> Example:
>
> ![ST-Link JTAG to SWD Adapter](./adapter-image.png)

---

## 📍 Pin Details

All pin names are printed on the PCB. Here's a reference for the minimum required:

- **4 Pins** (1, 2, 3, 4) — For programming
- **6 Pins** (1, 2, 3, 4, 5, 6) — For full debugging + programming

---

## 🔌 Jumper Connection Info

When using with different ST-Link versions:

- **Genuine ST-Link V2 or V3**:  
  Connect `VTarget (VTr)` to the target board's `VDD`.

- **Clone ST-Link (e.g. Chinese versions)**:  
  Connect the adapter's **3.3V** pin to the target's `VDD`.

---

## 📦 Specifications

| Attribute       | Value       |
|----------------|-------------|
| Dimensions      | 30 mm x 31 mm |
| Connector Type  | ARM 20-pin JTAG to SWD Header |
| Programmer Support | ST-Link, J-Link, and others |

---

## ✅ Compatibility

| Programmer | Compatible |
|------------|------------|
| ST-Link V2 | ✅ |
| ST-Link V3 | ✅ |
| J-Link     | ✅ |
| Other JTAG headers | ✅ |

---

## 📁 Gerber Files

The `gerber/` directory contains the production-ready files for PCB manufacturing.

Inside this folder, you will also find a `panelization/` subfolder — this is the version used for panelized PCB manufacturing via **JLCPCB**. You can directly upload this to JLCPCB’s order page to manufacture your board.

---

## 📝 License

This project is released under the [MIT License](LICENSE).

---


