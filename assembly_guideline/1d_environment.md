---
title: "Environment and Tools"
excerpt: ""
permalink: /education/reproduction_environment/
---

- Prepare tools and place
-> foto of each part
  - table
  - crimping tool
  - screwdriver
  - side cutter
  - allen wrench
- Prepare material and components
  - Frame and Housing (in this case UniProKit)
    - screws, nuts
    - T-slot alu profile
    - 3D printed corner elements / connectors
    - bottom plate
    - housing plates
  - Battery pack
    - 3D printed battery case (bottom and cap -> download link to file)
    - battery cells
    - cell connectors
  - electrical components
    - Libre Solar components -> MPPT, *BMS*, (optional: CAN2Wifi)
    - (optional: RaspberryPi0)
    - wires - power wires (6 sq mm), balancing wires (2 sq mm)
    - ferrules, cable lugs
    - (optional: communication wire - ethernet cable)
   - plugs
     - *dc-output plugs (car plug, 2x)*
     - solar input plugs (Weidmüller PV Stick allows assembly w/o crimping and is compatible to MC4. Clips should be removed that the plug can be unmounted without tools)
     - *usb plugs*
     - *ON/OFF switch, pushbutton, integrated LED*
     - (optional: RJ45 jacks (2x))
     - (optional: epaper display+conncetion wire)

------------------------------------------------------

The Libre Solar project files are all open source and [stored on GitHub](https://github.com/LibreSolar). There is a separate repository for each PCB and an additional repository for the software.

Some of the repositories contain git submodules, so please use
```
git clone --recursive <repository>
```
instead of the download button on github.


## Hardware design

Except for some old boards, all Libre Solar electronics hardware is built using the open source PCB design software [KiCad 5](http://kicad-pcb.org/).

As KiCad version 5 contains lots of interesting new features (better rendering, rounded pads, STEP export, better symbol file format), the Libre Solar PCBs were recently converted to this version. Unfortunately, the files are not compatible with the older KiCad version 4 anymore. Please download the nightly builds or the stable KiCad version 5 as soon as it is released.

Custom footprints and symbols are saved in separate repositories:

- [https://github.com/LibreSolar/KiCad-footprints](https://github.com/LibreSolar/KiCad-footprints)
- [https://github.com/LibreSolar/KiCad-symbols](https://github.com/LibreSolar/KiCad-symbols)

The footprint library is directly included via the github import feature in KiCad. This feature does not exist for the schematics editor, so the schematic symbols are included via a git submodule.

## Software development

The firmware for the Libre Solar hardware is developed using the [ARM mbed OS](https://developer.mbed.org/) embedded software framework. This makes it possible to use easy-to-understand C++ syntax (similar to Arduino) and enhances community based software development.

We recommend to use Visual Studio Code and [PlatformIO](http://platformio.org/) as an IDE for software development.

All Libre Solar software repositories are structured as PlatformIO projects:

```
|--lib/
|  |--Foo
|  |  |- Foo.cpp
|  |  |- Foo.h
|  |--Bar
|  |  |- Bar.cpp
|  |  |- Bar.h
|--src/
|  |- config.h
|  |- main.cpp
|- platformio.ini
|- README.md
|- LICENSE
```

The main firmware is located in the `src` folder, external libraries or reuseable code are stored under `lib`.

The platformio.ini file contains some important settings which might have to be adjusted:

```ini
[env:nucleo]
platform = ststm32
framework = mbed
board = nucleo_f072rb
upload_protocol = stlink

# Settings:
# - enable float formatting for printf, adding approx. 7 kB of bin file size
# - C++11 to be able to define default values for struct members
# - Use low speed internal clock (LSI) for RTC (no LSE crystal on PCB)
build_flags =
    -Wl,-u_printf_float
    -std=c++11
    -DMBED_CONF_TARGET_LSE_AVAILABLE=0

# Custom Serial Monitor port
# monitor_port = /dev/ttyUSB1

# Custom Serial Monitor baud rate
monitor_baud = 115200
```

Of course, you can also use your favourite IDE and the mbed command line interface.

The chapter **Flashing** describes in detail how you connect the hardwar in order to upload the software to the device.
