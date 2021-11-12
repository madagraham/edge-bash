# IoT Edge Device Config Automation

To automate the configuration of IoT edge devices prior to field deployment, I created a Bash script for technicians to utilize during the hardware configuration process. Said Bash script must be run 6 times to successfully configure the edge device.  Each time the script is run, a file called `reboot` is created (i.e. `reboot1`, `reboot2`, etc.). Once the script is run 6 times, and the device is successfully configured, all `reboot` files are automatically deleted. 

> **Note:** This Bash script is intended to be used on IoT edge devices with 
> a [Clear Linux OS](https://docs.01.org/clearlinux/latest/get-started/bare-metal-install-server.html#download-the-latest-cl-live-server-image).