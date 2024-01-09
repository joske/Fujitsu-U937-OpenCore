# Fujitsu Lifebook U937

OpenCore config for this ultra light laptop containing:

- i5 7200u iGPU UHD 620
- 13 inch FHD touchscreen (touch disabled in BIOS)
- 20 GB RAM
- 1 TB WD Blue NVMe SSD (half for Linux, half for macOS)
- Intel wifi
- Intel I219LM4 ethernet
- bluetooth - BCM_4350C2
- dual boots with linux

## What works

- Boots fine into macOS Ventura
- Power Management
- Video acceleration - metal 3
- brightness control via control center slider
- volume keys
- touchpad + gestures
- Onboard audio using layout id 3 (USB & HDMI audio also work)
- sleep/wake
- onboard WiFi works with AirportItlwm.kext
- onboard ethernet with IntelMausi.kext
- USB hotplugging
- webcam (UVC Camera VendorID_1266 ProductID_46566)
- HDMI output works, after unplugging, the internal display is dark for a while, but comes back

## What doesn't work

- bluetooth is detected, but doesn't turn on, don't care enough to troubleshoot
- Card reader (Alcor 9540) - lost cause, unsupported, no problem, works in linux
- brightness keys
