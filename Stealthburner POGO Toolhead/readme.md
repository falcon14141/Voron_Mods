# **POGO Toolhead Mod for the Voron Stealthburner**

This will allow rapid toolchange of the Voron Stealthburner toolhead by removing the need of plugging and unplugging the toolhead.
Both extruder power, and temperature sensor are connected using pogo pins.

**Beware: This mod requires soldering skills**

![pogo toolhead on CW2](images/Pogo-CW2.png)
![pogo toolhead Dragon & Revo](images/collection_front.jpg)
![pogo toolhead Dragon & Revo](images/collection_top.jpg)

## Mounting options

Though the principle may be the same, the PCB allows for several variations of the mounting, depending on your personnal usecase

1. *1 pair of pogos for the hotend, 2 pairs for temperarature sensor*

    I have toolheads with either a standard temperature sensor, or a PT100/PT1000. As they will have to connect to different pins of the MCU, I chose to have both prewired on the extruder pcb, and solder either TH0 or TH1 on the toolhead PCB depending on my specific toolhead
2. *2 pairs of pogos for the hotend, 1 pair for temperature sensor*

    I you want to double the power troughput to the hotend, you can also bridge the HE and TH1 pogos together while soldering, and only use TH0 for the temperature sensor.
If you install a header on the extruder PCB, you may still have to option to swtich from thermistor to PT100/PT1000 if required

## Assembly instructions

![toolhead assembly parts](images/toolhead-assembly.jpg)

Use the provided toolhead helper to solder the toolhead pogo. This will ensure the right placement of the pogo on the PCB, since this in not a conventional mounting option.

Use heatshrink on the cable, to avoid the risk of short-circuit between wires.

Once the toolhead pcb has been soldered, insert it in the groove of the back part. Once the front part has been mounted, the pcb should not be able to move

On the extruder side, slide the PCB in place, and secure it using a flathead M3 screw.
## BOM

It is important to wisely chosse the pogo pins, as the extruder power needs to go through the pogo. I chose models made by Mill-Max as they have been certified up to 3A current on a single pin.

- Toolhead pogo : Mill-Max 827-22-006-10-001101
- Extruder pogo : Mill-Max 419-10-206-00-006000 
- 2p PCB header
- 1x M3x10mm screw to hold the extruder PCB

For the LGX Lite extruder mount:
- BOM as stated on https://github.com/Eytecz/LGX_Lite_Stealthburner_CW2_style_mount

For the LGX extruder mount:
I liked the deisgn made by Eytecz for the LGX Lite, and made a smiliar mount for the LGX.
- 2x M3x22mm screws for the bottom mount of the LGX
- 1x UM2 collet.

## Making new Toolheads

The CAD inludes some parts that can be added or trimmed from other SB toolheads to make them compatible to this mod. For a skilled F360 user, it should be quite easy to use.


## Authors

- falcon14141

