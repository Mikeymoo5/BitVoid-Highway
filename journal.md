---
title: "BitVoid Handheld"
author: "@Michael, @Elly"
description: "A handheld retro console powered by an RPI Zero 2W"
created_at: "2025-06-27"
---
## Initial Setup
@Michael
The initial git commit ads KiCad files that consist solely of the schematics for a USB-C receptacle and an RPI Zero 2W.
**Time**: 0.16 hours

## Battery Charger
@Michael
I worked a bit more on wiring the battery charger. I chose a TI BQ25308 charger, since from what I can tell it fits our needs (5V3A input, and 4.2V output) while still being decently efficient. 

After looking through the datasheet for the charger, I configured it to output 4.2V, the maximum battery voltage of the batteries we plan on using.

**Time**: 0.16 hours

## Controls
@Michael
Over the course of a few days, we have been researching joysticks, screens, buttons, and ADC's (for use with the two joysticks). We decided on the TI ADS1115IDGSR, particularly for its cheap price and 4 lane input. We also wanted it to use an easy communication protocol, and this one supports I2C.

I began implementing the controls, the ADC for the joysticks, and split some of the general functions into seperate schematic sheets.
**Time**: 1.25 hours