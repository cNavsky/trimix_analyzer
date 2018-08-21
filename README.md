# trimix_analyzer
DIY Trimix Analyzer

Caveats

This is experimental project to satisfy one's curiusity. Build at your own risk, don't rely for life support operations, get proper traning before using gas mixes etc. 

Inspiration

This is loosely based on captainigloo project:
https://github.com/captainigloo/Trimix-analyzer
Which, in turn, based on Monsieur Yves Cazé design.

Design

My main design goal was to simplify and improve. Here are the basic differences:
    1. I decided to use VQ546MR Sensor module from Sensortech. First, because it have proper documentation, readily available via Digikey and Mouser and have known quality.
    2. Reading sensor datasheets it became clear that for measuring HE snsor heater temperature is not critical, it actually a little more sensitive at lower temps. As such, we can use nuch less power and get away without separate power supply.
    3. Arduino used is Adafruit M0 module (they have several, any will do). It's 3v based, have powerful onboard linear regulator (power supply), and li-ion charger controller.
    4. Screen is Adafruit Monochrome 1.3" 128x64 OLED graphic display.
    5. O2 sensor cell is from JJ Rebreather. Because we have a limitless supply of used cells :-). Pretty much any rebreather of O2 analyzer cell will work.
    6. Added button interface for control.
    7. Added optionsl temperature/humidity sensor for O2 calibration.
    8. Code have startup and on-demand calibration routines and provisions for storing calibration data in non-volatile memory.
    9. This design can be used as a O2 analyser only.

Versions

There will be 2 main versions. 
One simple, from readily available components which requires minimum soldering. It can be powered by 1 li-ion cell or 3 AA cells. 
Advanced integrated version with purposely sesigned pcb, one button interface for power (with timed power down), powered by 1 Li-ion cel.

To be continued.
