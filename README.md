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
* Baudrate 115200

### Configuration-FULLGRAPHICSDISPLAY.h 
This is my initial (fully working) example configuration for a Reprapdiscount Full Graphic Smart Controller display with the following settings:
* RepRapDiscount Full Graphic Smart Controller 128x64 (FEATURE_CONTROLLER 11)
* Slowest UI Encoder Speed (UI_ENCODER_SPEED 2)
* Disabled Allows faster value selection by turning encoder faster. (UI_DYNAMIC_ENCODER_SPEED 0)
* Correct (reversed) scroll direction (UI_REVERSE_ENCODER 1)

The buttons seem to be working fine and there was no need to include any graphic library.

Still to be tested/implemented:
* autolevel feature, that's a work in progress
* filament runout feature

#### Using and flashing
You can use this Configuration.h in the dev version of the Repetier configurator to finetune and download a complete firmware source package:

https://www.repetier.com/firmware/dev/index.php

The firmware can be flashed using ArduinoIDE:

https://www.arduino.cc/en/main/software

With the following board settings:
* Board type: "Arduino/Genuine Mega or Mega 2560"
* Processor type: "ATmega2560 (Mega 2560)"
* Baudrate 115200