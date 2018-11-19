# HA-Thermostat

## Home Assistant Thermostat Packages - Generic Thermostat Component ##
Both of these packages are for a dual unit home, but could be modified easily

Both packages include mode and disable switches that sets both thermostats, can be controlled via alexa etc, and is retained during restarts!
I always hated I lost my modes on restarts, and had to edit yaml when the climate changed.

### Automations ###

Set all systems to cool or heat on start/restart based on mode selection.

Set all systems to cool or heat when mode selection is toggled.

Disable all systems - Windows open, service etc.

**future: Notify phone if window open states (konnected) with systems running

**future: Actionable Notification to disable systems, or ignore

**future: Restore systems once windows are closed again

Restore all systems based on mode selection

These automations affect both units and sets all 4 thermostats

IMPORTANT - Both packages include an automation to prevent both AC and Furnace from being called at the same time!

### Files ###
"thermostat.yaml" is the standard setup, 2 sets of control devices with 3 relays each...AC, Furnace, Fan
includes the above automations, and fan control (call fan with AC)

"thermostat_4ch_no_fan.yaml" is all of the above goodies but adjusted to run a dual unit home with a sonoff 4ch, no manual fan control! (my setup)
https://youtu.be/hOFvbdYkOII - great video on flashing the 4chpro...I got it forst try with tasmota 6.2.1
https://github.com/arendst/Sonoff-Tasmota/wiki/Sonoff-4CH-and-4CH-Pro - see bottom for dipswitch settings


