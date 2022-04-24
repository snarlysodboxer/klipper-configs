# Klipper on Azteeg X5 GT with TMC2660 steppers

This is for my Pulse XE from Matterhackers

## Status
Accelerometers installed for input shaping calibration
This setup is working really nicely with the master branch of Klipper

Notes:
I calculated these stepper_ settings using the register settings from the smoothieware config, however not all settings smoothieware was setting are supported by Klipper. I opted to let Klipper configure it's defaults.
```yaml
driver_TBL: 3
driver_RNDTF: 0
driver_HDEC: 0
driver_CHM: 0
driver_HEND: 3
driver_HSTRT: 4
driver_TOFF: 0
driver_SEIMIN: 0
driver_SEDN: 0
driver_SEMAX: 0
driver_SEUP: 0
driver_SEMIN: 0
driver_SFILT: 0
driver_SGT: 0
driver_SLPH: 0
driver_SLPL: 0
driver_DISS2G: 0
driver_TS2G: 0
# SET_TMC_FIELD STEPPER=stepper_x FIELD=DEDGE VALUE=0
```
