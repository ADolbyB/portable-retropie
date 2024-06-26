# Portable RetroPie Config Files

Here I place my working config files for my RetroPie.

My RetroPie is a work in progress with many parts I already had sitting around.
I will share details of this easy build here.

## Features:

- 10 inch HDMI LCD screen.
- Raspberry Pi 3B+ running the Buster release of Retropie.
- Wireless controllers and keyboard.
- Fully portable: needs only a USB-A power connection.

## Components:

- 1x RPi 3B+ (v1.2) with the latest RetroPie image.
- 1x RPi 3B+ Case (Choose One you like).
- 1x [HD 10.1" TouchScreen](https://www.amazon.com/dp/B0CJNKFVPY?th=1)
    - This kit comes with a new power supply and a bunch of cables for the power and touchscreen.
    - This screen can be powered directly by the RPi 5V & Ground GPIO, thereby only needing
- 1x [Wireless Keyboard](https://www.amazon.com/dp/B098WTHSYR)

## Build Pics:

- Note that this is a work in progress. When I get a 3D printer, I would like to create a better stand/case with a handle for easy travel.

<div align="center">

<p>Front View:</p>
<img src="./RPi-3B+/assets/RPi_Front.jpg" alt="Front" width="600"/><br><br>
<p>Rear View</p>
<img src="./RPi-3B+/assets/RPi_Rear.jpg" alt="REAR"width="600">

</div>

### Notes on Config Files:

- `config.txt` has the following file location: `/boot/config.txt`
    - Used for Overclocking, Turbo Mode and Over Voltage.
    - File Setting Sources Used: 
        - [RPi Docs: BCM2837B0 Processor Specs](https://www.raspberrypi.com/documentation/computers/processors.html#bcm2837b0)
        - [RPi Forum: Pi 3B Overclock Settings](https://forums.raspberrypi.com/viewtopic.php?t=235753)
        - [RetroPie Forum: Overclocking the Pi3B+ GPU](https://retropie.org.uk/forum/topic/21138/overclocking-the-pi3b-gpu-results/2)
        - [RPi Docs: `raspi-config` settings](https://www.raspberrypi.com/documentation/computers/configuration.html)
        - [RPi Forum: Undervoltage on the Pi3](https://retropie.org.uk/forum/topic/1006/under-voltage-on-the-pi3/5)
- `es_systems.cfg` has the file location: `/etc/emulationstation/es_systems.cfg`
    - Used for displaying the names and logos of each game console in Emulation Station.
    - This file is modified for the US with the Sega Genesis logo.
- `retroarch-core-options` is used to set the core settings for the ROM and Emulator.
    - This is my working file.