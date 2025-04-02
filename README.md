
1. install openvm on a clean ubuntu vm and reboot

sudo apt install open-vm-tools -y && sudo apt install open-vm-tools-desktop -y

2. download and unzip the v2raylove

   cd ~/Desktop && \
wget -O ~/Desktop/20250402.tar.gz https://github.com/redlock163/v2rayLOVE/archive/refs/tags/20250402.tar.gz && \
tar -xzvf ~/Desktop/20250402.tar.gz -C ~/Desktop && \
cd ~/Desktop/v2rayLOVE-20250402 && \
tar -xzvf v2rayLOVE-20250402.tar.gz -C ~/Desktop/v2rayLOVE-20250402 --strip-components=1 && \

rm -rf ~/Desktop/v2rayLOVE-20250402/v2rayLOVE-20250402 && \
rm ~/Desktop/v2rayLOVE-20250402/*.gz

4.
python3 get_os_and_modules.py 

python3 install_tkinter.py 



