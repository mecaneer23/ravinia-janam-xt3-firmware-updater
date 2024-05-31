# Janam XT3 Scanner Firmware Updater

Automatic firmware upgrade script for Janam XT3 Scanner. Developed for Ravinia Festival.

## Required hardware

- Janam XT3 Scanner (Android)
- Windows computer with administrator permissions
- USB-A to USB-C wire (or another cable which can connect a computer to the scanner)

## One-time setup

- Download and unzip [scanner driver](https://developer.android.com/studio/run/win-usb)
- Download and unzip [fastboot firmware package](https://janam-assets.azureedge.net/assets/XT3/FSBT/91.16_20231011.zip)
- Download and install [AutoIt windows automation software](https://www.autoitscript.com/files/autoit3/autoit-v3-setup.zip)
  - Make sure that default double click behavior is `run` rather than `edit`
- Clone or download this GitHub repository

## Per-scanner usage

### Get scanner ready

- Put scanner into fastboot mode
  - Turn scanner off
  - While holding volume down + home, press and hold power button until fastboot screen is visible (do not advance past this screen)
- Connect scanner to computer using wire

### Update scanner driver

#### Manually

- Open `devices and printers`
  - In control panel, select `View devices and printers` beneath `Hardware and Sound`
- Ensure scanner is visible as `Android` in device list (you might need to scroll down)
- Select the scanner (double click)
- Click `Hardware` at the top &#8594; `Properties` or double click `Android` under `Name` &#8594; `Change Settings` &#8594; `Update Driver...` &#8594; `Browse my computer for drivers` &#8594; `Let me pick from a list of available drivers on my computer` &#8594; `Show All Devices` &#8594; `Have Disk...` &#8594; `Browse...`
- Navigate to the file in the usb_driver folder called `android_winusb.inf`, click on it, then press `Open`
- Press `OK`
- Double click `Android Bootloadeer Interface` - it should be the middle option
- Click `Yes` &#8594; `Close` &#8594; `Close` &#8594; `OK`

#### Automatically

- Double click `update_driver.au3`

### Update scanner firmware

- Double click `RunThis.bat` in firmware folder
- Wait for process to finish and scanner to reboot
- Press any key to close the command prompt window

### Clean up

- Disconnect scanner from computer
- Setup scanner, skipping everything until device is fully on
- Sign into Google account
