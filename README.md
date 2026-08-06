# Adjustable DC-DC Step-Down Converter

This project demonstrates the design and implementation of an adjustable DC-DC buck converter using the **LM2596S-ADJ** IC. The converter accepts a wide input range of **4.5–40V DC** and delivers a regulated, adjustable output capable of supplying up to **3A** continuous current.

## Features

- Complete schematic design in KiCad
- LTspice simulation for stability and performance verification
- Optimized PCB layout for high efficiency and low output ripple
- Power stage, feedback network, and input/output filtering included
- Reliable voltage regulation using feedback compensation techniques

## Specifications

| Parameter | Value |
|---|---|
| IC | LM2596S-ADJ |
| Input Voltage | 4.5V – 40V DC |
| Output Voltage | Adjustable |
| Max Output Current | 3A (continuous) |
| Topology | Step-down (Buck) |

## Repository Contents

```
├── KiCad/          # Schematic and PCB layout files
├── LTspice/        # Simulation files for stability and performance analysis
└── README.md
```

## Design Overview

The converter is built around the LM2596S-ADJ switching regulator, configured with an external feedback resistor divider to allow adjustable output voltage. The design includes:

- **Power stage** — inductor, diode, and switching components sized for target load current
- **Feedback network** — resistor divider with compensation for stable regulation across the input range
- **Input/output filtering** — capacitor selection for ripple reduction and stability margin

## Simulation

LTspice simulations were used to verify loop stability and steady-state performance prior to PCB fabrication, validating transient response and output ripple against the design targets.

## PCB Layout

The PCB layout follows standard buck converter layout guidelines — minimized switching node area, tight power loop, and proper ground return paths — to reduce EMI and ripple while maximizing conversion efficiency.

## Tools Used

- **KiCad** — Schematic capture and PCB design
- **LTspice** — Circuit simulation and stability analysis

## License

Feel free to specify a license (e.g., MIT) if you'd like others to reuse this design.
