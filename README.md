# EMU Audity 2000 Upgrade

Community-provided updater for the E-mu Audity 2000 synthesizer. Provides a ROM-based upgrade path and diagnostic tools. Distributed as-is for non-commercial use only. No derivatives. Use at your own risk.

# E-mu Audity Updater

© 2026 Ray Bellis

---

## Important

This updater is offered to the community **as is**, with **no warranty**.

It has been tested on several Audity 2000 units without issue.  
Its use is **entirely at your own risk**, and the author will not be responsible for any failure or damage to your device.

In the (unlikely) event of a failure, **UK users are welcome to visit the author in person for assistance**.

---

## Instructions

### Before you begin

- **Back up your user presets!**

---

### Hardware preparation

- Program the desired updater version into an **AM29F040B PLCC32 NOR Flash IC**.  
  These are widely available and typically cost around **$1 USD**.

- With the Audity 2000 **powered off**, insert the programmed **AM29F040B** into **U13**, the (usually empty) **PLCC32 socket** located at the **top right of the Audity 2000 PCB**.

  ⚠️ **Pay very close attention to chip orientation** and be careful during insertion.

- Place a **jumper across the two lower pins of W1**, labelled **“8”**.


### Jumper Configuration

![Audity 2000 W1 Jumper Location](https://raw.githubusercontent.com/findsp/emu-audity-2000-upgrade/refs/heads/main/images/picture-jumper.jpg)

### Upgrade ROM Socket (U13)

![Audity 2000 PLCC32 Socket Location](https://raw.githubusercontent.com/findsp/emu-audity-2000-upgrade/refs/heads/main/images/picture-socket.jpg)

---

### Running the updater

- Power on the Audity 2000 and observe it booting from the **upgrade ROM**.

- Once booted, the following menu options are available:

  1. Show current version  
  2. Show flash chip ID \[*\]  
  3. Install OS update  
  4. Dump OS to MIDI  

- A video demonstration of the upgrade process is available here:  
 [▶ Watch the upgrade demo on YouTube](https://www.youtube.com/watch?v=V7Mba2Qw8JA)

[![Ray Bellis – E-mu Audity 2000 Upgrade Demo](https://img.youtube.com/vi/V7Mba2Qw8JA/0.jpg)](https://www.youtube.com/watch?v=V7Mba2Qw8JA)


---

### After updating

- Power off the Audity 2000.
- Remove the **jumper**.
- Remove the **upgrade ROM**.

- On the next power-on:
  - NVRAM will be reset
  - Factory presets will be restored
  - Restore your user presets if desired

---

## Notes

\[*\] **Flash compatibility notice**

This update ROM currently supports **Intel or Micron 28F800 flash devices only**.

If your Audity 2000 contains **AMD flash memories**, please:

- Send a clear photo of the flash chips  
- Include the output from the **“Show flash chip ID”** screen  

You can find the author on Facebook in **most E-mu-related groups**.

---

## License

This project is licensed under the  
**Creative Commons Attribution–NonCommercial–NoDerivatives 4.0 International License (CC BY-NC-ND 4.0)**.

You may share this material with attribution for non-commercial purposes only.  
No derivatives or modifications are permitted.

Full license text:  
![License: CC BY-NC-ND 4.0](https://img.shields.io/badge/License-CC%20BY--NC--ND%204.0-lightgrey.svg)

---

## Attribution

Original work by: <a href="https://www.youtube.com/watch?v=V7Mba2Qw8JA" target="_blank" rel="noopener">Ray Bellis</a> ![License: CC BY-NC-ND 4.0](https://img.shields.io/badge/License-CC%20BY--NC--ND%204.0-lightgrey.svg)  
This repository redistributes the original, unmodified release
with permission granted under the original license.

