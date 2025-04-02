# Installation Guide for V2RayLOVE

This guide provides step-by-step instructions to install Open VM Tools, download and unzip the V2RayLOVE package, and run the necessary Python scripts on a clean Ubuntu VM.

---

## Steps:

### 1. Install Open VM Tools on a Clean Ubuntu VM and Reboot
Run the following commands to install Open VM Tools and reboot the system:
```bash

sudo apt install open-vm-tools -y && sudo apt install open-vm-tools-desktop -y
sudo reboot
```

---

### 2. Download and Unzip the V2RayLOVE Package
Follow these steps to download and extract the V2RayLOVE package. You can also copy and paste the entire block of commands below:

```bash
cd ~/Desktop && \
wget -O ~/Desktop/20250402.1.tar.gz https://github.com/redlock163/v2rayLOVE/archive/refs/tags/20250402.1.tar.gz && \
tar -xzvf ~/Desktop/20250402.1.tar.gz -C ~/Desktop && \
cd ~/Desktop/v2rayLOVE-20250402.1 && \
tar -xzvf v2rayLOVE-20250402.tar.gz -C ~/Desktop/v2rayLOVE-20250402.1 --strip-components=1 && \
rm ~/Desktop/v2rayLOVE-20250402.1/*.gz
```

---

### 3. Run the Python Scripts
After successfully extracting the V2RayLOVE package, run the following Python scripts:

```bash
python3 get_os_and_modules.py
python3 install_tkinter.py
```

### 4. Start V2Ray
```bash
python3 1.py
```

#### Additional Setup:
1. Open the V2Ray GUI.
2. Set the subscript link (if applicable).
3. Click "Update."
4. Enable "Proxy" and "Autostart."
5. Reboot the system:
   ```bash
   sudo reboot
   ```
