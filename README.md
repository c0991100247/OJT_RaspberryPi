# hardward overview
- instructor provides Raspberry Pi 5, power cord, and SD card
- prevent from short circuit, place the raspberry on paper


# PC software setup
![setup](202503221401.png)
- download from PC browser
- Device: choose "Pi 5"
- OS: choose latest 64-bit
- when clicking "Next", customize OS for this course
- device name pi+name
- user name "Pi"
- password "raspberry"
- enable wifi to classroom AP
- enable SSH in SERVICE tab

# Raspberry Pi initialization
- after mini SD (OS) is ready, insert to device
- connect to power

## on PC, simulate terminal *Warp*, an AI-based software
![instruction](202503221441.png)
- download from PC warp.dev [link](https://www.warp.dev/)
- signin is possible with Google account
- both PC (where Wrap is installed) and Raspberry Pi must connect to a same AP (wifi network)
- connect from PC to Raspberry Pi via SSH
- query for detail steps by asking question to Wrap AI
> how to connect my Raspberry Pi device via SSH?
- once connected, Wrap will display pi@piCYC0200
- connectino can also be made via other command-line environment, such as VSCode terminal
```
ssh pi@piCYC0200.local
```
- troubleshooting: reboot the Raspberry Pi, or format it and install again

## setup Raspberry Pi from terminal
- from terminal, call menu by
```
sudo raspi-config
```
- enable VNC (3)
- install languages en_GB, en_US, and UTF-8 at (5)
- configure time zone at (5)
- select WIFI country to TW at (5)
- run update (8)
- click `Finish`
