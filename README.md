
---

# RISC-V SoC Tapeout Program VSD

Welcome to my journey through the **RISC-V SoC Tapeout Program VSD**.
This repository documents my **week-by-week progress**, starting with environment setup and tool installation.

---

## Week 0 — Setup & Tools

| Task                          | Description                                                                                                            | Status |
| ----------------------------- | ---------------------------------------------------------------------------------------------------------------------- | ------ |
| [**Task 0**](week_0/README.md) | Installed essential open-source EDA tools (**Iverilog**, **Yosys**, **GTKWave**, **Ngspice**) and configured Ubuntu VM | Completed|

### Tools Installed

| Tool     | Purpose                            |Verification |
| -------- | ---------------------------------- |------------ |
| Yosys    | RTL Synthesis & Logic Optimization |Verified     |
| Iverilog | Verilog Simulation & Compilation   |Verified     |
| GTKWave  | Waveform Viewer                    |Verified     |
| Ngspice  | Analog & Mixed-Signal Simulation   |Verified     |

### VM Configuration

* OS: Ubuntu 20.04+
* RAM: 6 GB
* HDD: 50 GB
* CPU: 4 vCPU

**VirtualBox Guest Additions (Optional but Recommended):**

```bash
sudo apt update
sudo apt install build-essential dkms linux-headers-$(uname -r)
cd /media/<username>/VBox_GAs_7.1.8/
sudo ./autorun.sh
sudo reboot
```

Enables **window resizing, shared clipboard**, and improved graphics in the VM.



### Key Learnings from Week 0

* Installed and verified **essential EDA tools** successfully.
* Learned **basic environment setup** for RTL design and simulation.
* Prepared system for **upcoming RTL-to-GDSII experiments**.

---

## Acknowledgment

I thank [**Kunal Ghosh**](https://github.com/kunalg123) and the [**VLSI System Design (VSD)**](https://vsdiat.vlsisystemdesign.com) team for the opportunity to participate in the RISC-V SoC Tapeout Program.
Support from **RISC-V International**, **India Semiconductor Mission (ISM)**, **VLSI Society of India (VSI)**, and [**Efabless**](https://github.com/efabless) is gratefully acknowledged.

---
