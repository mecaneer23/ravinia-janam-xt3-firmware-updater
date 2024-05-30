# Janam XT3 Scanner Firmware Updater

Automatic firmware upgrade script for Janam XT3 Scanner. Developed for Ravinia Festival.

## Required hardware

- Janam XT3 Scanner (Android)
- Windows computer with administrator permissions
- USB-A to USB-C wire (or another cable which can connect a computer to the scanner)

## One-time setup

- Install and unzip [scanner driver](https://developer.android.com/studio/run/win-usb)
- Install and unzip [fastboot firmware package](https://janam-assets.azureedge.net/assets/XT3/FSBT/91.16_20231011.zip)

## Per-scanner usage

- Put scanner into fastboot mode
  - Turn scanner off
  - While holding volume down + home, press and hold power button until fastboot screen is visible (do not advance past this screen)
- Connect scanner to computer using wire
- Open `devices and printers`
  - In control panel, select `View devices and printers` beneath `Hardware and Sound`
- Ensure scanner is visible as `Android` in device list (you might need to scroll down)
- Select the scanner
- Click `Properties` &#8594; `Hardware` at the top &#8594; INCOMPLETE
