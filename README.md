# Fujitsu Lifebook U937 

OpenCore config for this ultra light laptop containing:

* i5 7200u
* 13 inch FHD touchscreen (touch disabled in BIOS)
* 20 GB RAM
* 1 TB WB Blue NVMe SSD (half for Linux, half for macOS)
* Intel wifi works out of the box with AirportItlwm.kext
* iGPU UHD 620
* dual boots with linux

## What works
* Boots fine
* Power Management
* Video acceleration
* brightness
* touchpad (but gestures are a bit wonky)
* Onboard audio using layout id 3 (USB & HDMI audio also work)
* sleep/wake
* USB WiFi Edimax 7822ULC (Using chris1111's driver at https://github.com/chris1111/Wireless-USB-Adapter)
* USB hotplugging
* webcam

## What doesn't work
* bluetooth - BCM_4350C2 is detected, but doesn't turn on, don't care enough to troubleshoot
* Card reader (Alcor 9540) - lost cause, unsupported, no problem, works in linux
* brightness keys
