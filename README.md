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

- Boots fine
- Power Management
- Video acceleration
- brightness control via control center slider
- volume keys
- touchpad + gestures
- Onboard audio using layout id 3 (USB & HDMI audio also work)
- sleep/wake
- onboard WiFi works with AirportItlwm.kext
- onboard ethernet with IntelMausi.kext
- USB hotplugging
- webcam (UVC Camera VendorID_1266 ProductID_46566)

## What doesn't work

- bluetooth is detected, but doesn't turn on, don't care enough to troubleshoot
- Card reader (Alcor 9540) - lost cause, unsupported, no problem, works in linux
- brightness keys
- HDMI output does something, but internal screen goes black and doesn't come back and external screen is corrupted

## Ventura issue

For some reason, when I try upgrading to Ventura, the upgrades b0rks and I have to reinstall Monterrey and restore from Time Machine.
