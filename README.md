# PMOD-quickstart

## USB and GPDI

Sugested way of connecting GPDI and USB PMOD is this:

![PMOD_USB_GPDI](pic/GPDI_USB.png)

### USB

As for the USB - this is the only way to connect it, as at TOP RIGHT corner ULX3S has 5V pins.

Be carefull when you connect other PMODS to that place!

### GPDI

As for the GPDI - GPDI IN is designed for this position as on this position we have all differential bidirectional pins gp[11:9],gn[11:9] allong differential clock capable pins gp[12],gn[12]

## OV7670

Sugested way of connecting OV7670 is this:

![PMOD_OV7670](pic/OV7670.png)

You can also test other ways of connection just be warned about TOP RIGHT 5V from ULX3S!

## Code: 

### USB

https://github.com/emard/ulx3s-misc/tree/master/examples/usb/proj/lattice/ulx3s/usbhid_host

Should output some HEX on OLED and onboard GPDI output

When you connect keyboard to US3 or US4 (or both) you should see some change...

### GPDI

GPDI OUT (you will need to adapt pins in lpf and top module)

https://github.com/emard/ulx3s-misc/tree/master/examples/dvi

GPDI IN (Use buttons to sync all signals (R,G,B,CLOCK))

https://github.com/emard/ulx3s-misc/tree/master/examples/dvi_in

### OV7670

https://github.com/emard/ulx3s-misc/tree/master/examples/ov7670_dvi/proj/ulx3s_ov7670_dvi

Should display camera picture on onboard GPDI output

If you need help, please let us know:

## Chat and support

### Discord chanel

    https://discord.gg/qwMUk6W (problems/question/general chat)

### Gitter chanel

    https://gitter.im/ulx3s/Lobby (Focused on development)
