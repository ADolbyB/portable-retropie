# Portable Raspberry Pi 3B+ (v1.2) Retropie. Notes on Config Files:

- `config.txt` has the following file location: `/boot/config.txt`
    - Used for Overclocking, Turbo Mode and Over Voltage.
    - File Setting Sources Used: 
        - [RPi Docs: BCM2837B0 Processor Specs](https://www.raspberrypi.com/documentation/computers/processors.html#bcm2837b0)
        - [RPi Forum: Pi 3B Overclock Settings](https://forums.raspberrypi.com/viewtopic.php?t=235753)
        - [RetroPie Forum: Overclocking the Pi3B+ GPU](https://retropie.org.uk/forum/topic/21138/overclocking-the-pi3b-gpu-results/2)
        - [RPi Docs: `raspi-config` settings](https://www.raspberrypi.com/documentation/computers/configuration.html)
        - [RPi Forum: Undervoltage on the Pi3](https://retropie.org.uk/forum/topic/1006/under-voltage-on-the-pi3/5)
        - [Raspberry Pi Memory Split](https://retropie.org.uk/docs/Memory-Split/)
        - [Increasing the Swap File on RPi](https://pimylifeup.com/raspberry-pi-swap-file/)
- `es_systems.cfg` has the file location: `/etc/emulationstation/es_systems.cfg`
    - Used for displaying the names and logos of each game console in Emulation Station.
    - This file is modified for the US with the Sega Genesis logo, and is located at
- `retroarch-core-options.cfg` is used to set the core settings for the ROM and Emulator.
    - This is my working file, located at `/opt/retropie/configs/all/retroarch-core-options.cfg`.
- `dphys-swapfile` has the file location: `/etc/dphys-swapfile`
    - This file is used to increase the swap memory from 100MB to 1.0GB.