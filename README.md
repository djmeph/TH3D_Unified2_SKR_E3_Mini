# TH3D_Unified2_SKR_E3_Mini
TH3D Unified2 Firmware for Ender 5 with Bondtech BMG Extruder

Key settings:

```
#define CUSTOM_ESTEPS_VALUE 415
#define REVERSE_E_MOTOR_DIRECTION
```

The Bondtech BMG has a 3:1 gear ratio and runs in reverse of the stock Ender extruder. 

Warning:

I have had this experience with TH3D firmware on both my Ender 3 with the original 8-bit controller and my Ender 5 with the SKR E3 Mini 32-bit controller.
On both firmware updates I was able to get the correct motor direction, but the ESteps value did not take. This can be fixed with a gcode command in the terminal.

```
M92 E415
M500
```
