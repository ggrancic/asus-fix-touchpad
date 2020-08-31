# asus-fix-touchpad

## Description
This is a bash script for load the Focaltech FTE1200:00 0B05:0201 Touchpad after suspending your machine.

## Installation
- Clone this repo and move to the **asus-fix-touchpad** folder.

- Get your touchpad module name with
`lsmod | grep i2c_hid`
(in my case that is the name of my touchpad module)

- Copy the **fixtouchpad** file to `/lib/systemd/system-sleep/`.

- The file should be executable. If not, run `chmod +x fixtouchpad`.

- Reboot your machine.

- Try suspending and waking your computer to test.
