# Half-Life Blueprint Flight Controller

A custom flight controller project focused on hardware blueprint design, routing, and embedded firmware architecture. This repository contains the complete KiCad hardware design files, component libraries, and scripts required to build the flight controller platform from scratch.

## Project Structure

```text
├── hardware/
│   ├── lib/                  # Custom LCSC 3D shapes, footprints, and schematic symbols
│   ├── easyeda.py            # Component conversion and utility script
│   ├── FlightController.kicad_pro   # KiCad project file
│   └── FlightController.kicad_prl   # KiCad project local settings
└── README.md
```

## Hardware Specifications & Components

The board utilizes high-performance, industry-standard components optimized for stabilization and power management:

*   **Microcontroller:** LQFP-64 package core processing unit handling layout routing and sensor loops.
*   **Sensors & Telemetry:** 
    *   **BMP580:** High-accuracy barometric pressure sensor (LGA-10) for precise altitude hold.
    *   **IMU:** 14-pin low-noise Inertial Measurement Unit (LGA-14) tracking pitch, roll, and yaw rates.
*   **Power Management:** TPS63070RNMR high-efficiency buck-boost converter (VQFN-HR-15) ensuring stable voltage regulation during voltage drops.
*   **Connectivity & Storage:** 
    *   USB-C interface for configuration, flashing, and debugging.
    *   MicroSD Card Slot (TF-SMD) for onboard blackbox flight logging.

## Getting Started

### Prerequisites

To view and modify the hardware blueprints, you will need:
*   [KiCad v7.0 or newer](https://kicad.org)
*   Python 3.x (to run the custom hardware automation scripts)

### Installation & Setup

1. Clone the repository to your local machine:
   ```bash
   git clone https://github.com
   cd FlightController
   ```

2. Open the project in KiCad:
   * Launch KiCad.
   * Click **Open Project** and select `hardware/FlightController.kicad_pro`.
   * The global and local footprint libraries (`fp-lib-table`) will load automatically.
  
3. <img width="680" height="625" alt="Screenshot 2026-11-07 210710" src="https://github.com/user-attachments/assets/4c1cd94b-420b-458d-ad7d-716c9755c410" />


