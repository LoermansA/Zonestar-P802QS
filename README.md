# Zonestar-P802QS
Files related to the Zonestar P802QS 3D printer, such as Configuration.h for the Repetier 1.0-dev firmware

### Configuration.h
Contains my settings for the 1.0.0.dev version of the Repetier firmware with the following properties:
* Zrib V3.0 board (should also work for Zrib V2, but that is not tested)
* Working keys and beeps
* Working SDCard reader
* Inverted X and Y steppermotors direction
* Heated bed
* 2 fans; one for the hotend and one for cooling the filament

Everything seems to be working fine, except the autolevel feature. That's a work in progress. I haven't tested the filament runout feature yet.

#### Using and flashing
You can use this Configuration.h in the dev version of the Repetier configurator to finetune and download a complete firmware source package:

https://www.repetier.com/firmware/dev/index.php

The firmware can be flashed using ArduinoIDE:

https://www.arduino.cc/en/main/software

With the following board settings:
* Board type: "Arduino/Genuine Mega or Mega 2560"
* Processor type: "ATmega2560 (Mega 2560)"