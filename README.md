# asus-fix-touchpad

## Description
This is a bash script to load the Focaltech FTE1200:00 0B05:0201 Touchpad after suspending your machine.

## Installation
- Clone this repo and move to the **asus-fix-touchpad** folder.

- Get your touchpad module name with
`lsmod | grep i2c_hid`
(in my case that is the name of my touchpad module)

- Copy the **fixtouchpad** file to `/lib/systemd/system-sleep/`.

- Replace `i2c_hid`for your touchpad module name in the script.

- The file should be executable. If not, run `chmod +x fixtouchpad`.

- Reboot your machine.

- Try suspending and waking your computer to test.

- You can forward all of the above steps by runing the bash script included in this repo (except getting the name of the module, i will try to fix that in the future).
