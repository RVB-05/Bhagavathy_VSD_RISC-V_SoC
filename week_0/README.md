# SFAL VSD Tools Installation and Setup

## Project Overview
This repository documents the installation and setup of essential tools for the SFAL VSD (Very Small Design) course. It includes step-by-step instructions, snapshots of successful installations, and verification commands for all tools.

---

## System Requirements
- RAM: 6 GB  
- HDD: 50 GB  
- CPU: 4 vCPU  
- OS: Ubuntu 20.04+  

VirtualBox Guest Additions (Optional but Recommended):
```bash
sudo apt update
sudo apt install build-essential dkms linux-headers-$(uname -r)
cd /media/<username>/VBox_GAs_7.1.8/
sudo ./autorun.sh
sudo reboot

```
This allows window resizing, shared clipboard, and improved graphics in the VM.
---

## Tools Installed

### 1. **Yosys**
Yosys is an open-source synthesis tool for digital circuits.

**Installation Commands:**
```bash
sudo apt-get update
git clone https://github.com/YosysHQ/yosys.git
cd yosys
sudo apt install make build-essential clang bison flex \
libreadline-dev gawk tcl-dev libffi-dev git graphviz xdot pkg-config python3 \
libboost-system-dev libboost-python-dev libboost-filesystem-dev zlib1g-dev
make config-gcc
make
sudo make install
```
![Yosys Installation](screenshots/Yosys_installation.png)

### 2. **Icarus Verilog (Iverilog)**
Iverilog is a Verilog simulation and synthesis tool.

**Installation Commands:**
```bash
sudo apt-get update
sudo apt-get install iverilog

```
![Iverilog Installation](screenshots/iverilog_installation.png)

### 3 **GTKWave**
GTKWave is a waveform viewer for simulation outputs.

**Installation Commands:**
```bash
sudo apt-get update
sudo apt install gtkwave

```
![GTKWave Installation](screenshots/gtkwave_installation_proof.png)
![GTKWave Installation proof](screenshots/gtkwave_proof_2.png)

### 4 **Ngspice**
Ngspice is a mixed-signal electronic circuit simulator.

**Installation Commands:**
```bash
# Download tarball from https://sourceforge.net/projects/ngspice/files/
tar -zxvf ngspice-37.tar.gz
cd ngspice-37
mkdir release
cd release
../configure --with-x --with-readline=yes --disable-debug
make
sudo make install

```
![Ngspice Installation](screenshots/ngspice.png)

### 5. **Magic VLSI**
Magic is an open-source VLSI layout editor and verification tool, widely used for designing, simulating, and analyzing integrated circuit layouts.

**Installation Commands:**
```bash
sudo apt-get install m4 tcsh csh libx11-dev tcl-dev tk-dev libcairo2-dev \
mesa-common-dev libglu1-mesa-dev libncurses-dev
git clone https://github.com/RTimothyEdwards/magic
cd magic
./configure
make
sudo make install

```
![Magic Installation](screenshots/magic_installation_proof.png)


