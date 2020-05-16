# whb04
Whb04b python driver for LinuxCNC

Installation:
- sudo apt-get update
- sudo apt-get install pip
- sudo pip install pyusb
- chmod +x ./whb/whb04b
- Create file /etc/udev/rules.d/90-xhc.rules and add a line in it:
        SUBSYSTEM=="usb", ATTR{idVendor}=="10ce", ATTR{idProduct}=="eb93", MODE="666" 
- sudo udevadm trigger
