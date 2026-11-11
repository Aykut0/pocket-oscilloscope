# Pocket Oscilloscope

A pocket-sized, battery-powered oscilloscope board built around an ESP32-S3. PCB design project.

![3D render of the board](docs/images/board_3d.png)

The probe input goes through a protected front end (a Schottky clamp to the rails) into op-amp buffer and scaling stages, with a switch for the input range so both small and larger signals fit the ADC. An ESP32-S3-MINI-1 module digitizes the signal, and its USB and wireless links can carry the waveform to a computer or phone. A single-cell LiPo with an on-board USB-C charger and a 3.3 V regulator lets it run untethered. Reset and boot buttons, status LEDs and test points are there for bring-up.

![Schematic overview, rendered from the KiCad file](docs/images/schematic_overview.png)

## Files

```
hardware/                 KiCad project (open pocket_oscilloscope.kicad_pro)
hardware/fabrication/     Gerber files
docs/images/              render and schematic
```

Open the project in KiCad 8 or newer. Some parts use the KiCad PCM "AKL" libraries; install them from the Plugin and Content Manager if symbols show as missing.

The board design and fabrication files are complete. Firmware is not part of this repository yet.

---

Yaşar Aykut Altuntop · Koç University · [LinkedIn](https://linkedin.com/in/aykutaltuntop) · [GitHub](https://github.com/Aykut0)
