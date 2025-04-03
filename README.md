# PrivTag: Low-Power Lost Device System

Mauricio Serrano & Sumukh Murthy

PrivTag is an energy-efficient, event-driven system designed to assist in locating lost devices.  
By integrating low-power timers, stop mode, and Bluetooth Low Energy (BLE), it achieves a system clock of 1 MHz while disabling non-essential peripherals.  
This design reduces power consumption to approximately 87 μA during idle periods and around 150 μA during BLE transmission, allowing the device to operate between ~55.6 to ~95.8 days on a single charge.  
In Lost Mode, PrivTag transmits real-time notifications via the NRF Toolbox to alert users.

---

## Features

- **Low Power Consumption:** Utilizes low-power timers and stop mode to minimize energy usage.
- **Bluetooth Low Energy Integration:** Enables efficient communication with user devices.
- **Real-Time Notifications:** Sends alerts through NRF Toolbox when the device is in Lost Mode.
- **Extended Battery Life:** Operates for approximately 55.6 to 95.8 days on a single charge.

---

## System Overview

PrivTag operates by entering a low-power idle state, consuming about 87 μA.  
Upon detecting a specific event (e.g., device loss), it switches to Lost Mode, activating BLE transmission at approximately 150 μA to send notifications via NRF Toolbox.

---

## Hardware Requirements

- Microcontroller supporting low-power modes and BLE functionality.
- Power source capable of sustaining extended low-current operation.

---

## Software Requirements

- [NRF Toolbox](https://play.google.com/store/apps/details?id=no.nordicsemi.android.nrftoolbox) application installed on the user's device.
- Firmware compatible with the microcontroller to manage low-power states and BLE communication.

---

## Installation and Setup

1. **Hardware Assembly:** Connect the microcontroller to the power source and ensure BLE functionality is enabled.
2. **Firmware Upload:** Flash the provided firmware onto the microcontroller.
3. **NRF Toolbox Configuration:** Install the NRF Toolbox app on your device and pair it with the PrivTag system.

---

## Usage

- **Normal Operation:** PrivTag remains in a low-power idle state to conserve energy.
- **Lost Mode Activation:** Upon triggering Lost Mode, the device transmits notifications via BLE to the paired device using NRF Toolbox.

---

## Power Consumption Details

- **Idle State:** Approximately 87 μA
- **BLE Transmission:** Approximately 150 μA
- **Battery Life Estimate:** Between ~55.6 to ~95.8 days, depending on usage patterns

---

## Contributing

Contributions to enhance PrivTag are welcome.  
Please fork the repository and submit a pull request with your improvements.

---

## License

This project is licensed under the [MIT License](LICENSE).

---

## Acknowledgments

Special thanks to the developers of NRF Toolbox for providing a reliable platform for BLE communication.

---

*For more information and to access the source code, visit the [PrivTag GitHub Repository](https://github.com/MauricioESerrano/-PrivTag-Low-Power-Lost-Device-System).*
