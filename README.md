# 51nb-X210-Hackintosh
Install macOS on your 51nb X210 frankenpads.

## Compatibility

**Motherboards**
- **2nd Batch with i5 8250U**: The main model this configuration was developed with and for.
- **Test/ 1st/ 3rd Batch with i5 8250U**: Compatible and tested.
- **1st/ 2nd/ 3rd Batch with i7 8550U** Compatible and tested.
- **1st/ 2nd/ 3rd Batch with i7 8650U** Compatible and tested.

**Screens**
- **Stock X200/ X201 WXGA Low-Res Display** Compatible and tested.
- **Stock X200s/ X201s WSXGA Hi-Res Display** Compatible and tested.
- **Stock X60/ X61 XGA Low-Res Display** Compatible and tested. This is for the X61HK mods only.
- **Stock X60T/ X61T SXGA Hi-Res Display** Compatible and tested. This is for the X61HK mods only.
- **X210 1920x1200 WUXGA Display** Compatible and tested.
- **X210 2880x1920 2K Display** Compatible in theory. Not tested.
- **X210 3000x2000 3K Display** Compatible and tested.
 
## Post-installation tweaks
A few required or otherwise useful steps to take on a running macOS system on your OneMix:

**Using your own serial number**

Just generate a new set with Clover Configurator and you're good to go

**Disabling Power-related Settings**

In order to achieve a stable sleep, you're responsible of disabling the following:
- Power Nap (if available)
- Wake for Internet Access
- tcpkeepalive (hint: `sudo pmset -a tcpkeepalive 0`)

**Brightness Control**

Use `Brightness Slider` from App Store. Partially works but it's inverted. Unfortunately native brightness control isn't supported at this moment, interested developers might want to take a look at the DSDT and PNLF.

## What works

- Full hardware acceleration
- Audio
- Battery reading and charging recognition
- USB-A ports
- CPU Temperature and voltage/wattage reading
- Internal Wi-Fi via OpenIntelWireless (Big Sur Support)
- Bluetooth via OpenIntelWireless
- Sleep
- Mini DP and VGA output

## What's untested

- Hibernation
- SD Card Reader
- Touchpad

## What's not yet working

- Native Brightness Control
- Native UltraNav Scrolling

## What will never* work

- Fingerprint

_* Not unless someone decides to make custom kexts for these, of course._
