# Micromanipulator_uM_NG

> ⚠️ **Disclaimer:** This is a preliminary hardware design and is currently **untested**. Use or produce these designs at your own risk.

**Micromanipulator_uM_NG** is a next-generation controller system designed for precision micromanipulation. It improves upon previous designs by introducing higher processing power, expanded I/O capabilities, reliable high-speed sensor communication, and comprehensive power monitoring.

## Acknowledgments & Prior Work

This project is the next-generation iteration of the original electronic system for [MicroManipulatorStepper](https://github.com/0x23/MicroManipulatorStepper) by [@0x23](https://github.com/0x23).
---

## Interactive KiCAD Design Viewers

You can inspect the schematics and PCB layouts directly in your browser without opening KiCAD, powered by [KiCanvas](https://kicanvas.org/):

* 🔗 **[View Sensor Board (MT6835 V1.0)](https://kicanvas.org/?repo=https%3A%2F%2Fgithub.com%2FAptustech%2FMicromanipulator_uM_NG%2Ftree%2Fmain%2FMT6835%2FV1.0%2FMT6835)**
* 🔗 **[View Controller Board (uM_Controller V1.0)](https://kicanvas.org/?repo=https%3A%2F%2Fgithub.com%2FAptustech%2FMicromanipulator_uM_NG%2Ftree%2Fmain%2FuM_Controller%2FV1.0%2FuM_Controller)**

---

## Key Features & Highlights

* **Powered by RP2350B:** Upgraded to the RP2350B microcontroller to leverage its high IO count and advanced processing capabilities.
* **High-Speed LVDS Link:** Uses Low-Voltage Differential Signaling (LVDS) lines between the main controller and sensor boards, enabling a high-speed, noise-resilient SPI bus operating at **15 MHz**.
* **Power & Diagnostics:**
  * **Input Voltage Monitoring:** Real-time tracking of the main supply voltage.
  * **Per-Motor Current Sensing:** Dedicated current monitoring for each individual motor driver channel.
* **Modular Expansion:** Includes an dedicated extension connector for easily adding custom interfaces, daughterboards, or peripheral modules.

---

## Hardware Repository Structure

```text
├── MT6835/
│   └── V1.0/          # MT6835 encoder/sensor board design files
└── uM_Controller/
    └── V1.0/          # Main RP2350B controller board design files
