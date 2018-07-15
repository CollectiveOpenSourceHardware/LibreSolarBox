# Assembly Workshop at the Fablab St.Pauli, 08. July 2018

### Preparation Steps
- Software tools
  - FreeCAD, 
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

Remarks: Parts in *italic font* still need to be ordered.

### Assembly Steps
1. Frame assembly
- 1.1 nuts into t-slot profile (

//comment from Oliver: fotos, which shows for each side the placement (and numbers) of the nuts (sitting in the slots). This is the key-information needed when assembling a box the first time, in order to avoid repeatedly re-opening the frame for adding some forgotten nuts


- 1.2 place profile in rectangle, place corner elements between profiles, screw together
- 1.3 repeat 
- -> result: 2 connected rectangle frame
- 1.4 connect the 2 rectangle frames with profile
- -> result: boxframe
2. screw bottom plate on bottom side of boxframe
- -> result: boxframe with bottom plate
3. cut and crimping wires
- 3.1 ...
4. battery pack assembly -> !!!!!safety note!!!!!
- 4.1 put battery cells in battery case (bottom part)
- 4.2 connect battery cells together
- 4.3 connect balancing wires with cells
- 4.4 connect power wires with battery cells
- 4.5 screw battery pack with bottom plate
5. mouting of electric components
...

### Disassembly Steps
1. remove blending parts (sides, backs)
-> pic box, mark sides, mark screws
2. remove fuse! -> no voltage/ current in system, note for electric safety rules 
-> pic fuse
3. remove interface (plugs, swith), by cutting, by 
-> pic interface, mark points to remove
4. remove cables from electric components
-> pic components, pic interface/jack
5. demount electric parts
-> pic screws
6. 


## Disassembly ##
### Disconnect BMS:
* Remove fuse.
* Remove BAT+ cable. 
* Mask metal end of the cable .
* Remove BAT- cable.
* Mask metal end of the cable.
* Remove PWR+ cables from BMS.
* Remove PWR- cables from BMS.
* Remove thin cables from BMS
* Remove internet cables from BMS.
* Remove monitor cables.
* Move ends of the cable down. Keep them away from batteries.
* Remove thin cables.

### Remove upper part of the case
* Remove screws from the upper blending.
* Remove screws from handles.
* Remove the upper blending with the handles.

### Remove interface blending
Interface are the sockets on the blending.

* Remove thick cables from blending if they are not soldered.
* Remove screws from the blending. Put them into a cup.
* Desolder on/off-swich.
* Remove CAN Socket.
* Remove USB power socket.
* Remove two DC Out 1V sockets.
* Do not remove PV INPUT and OUTPUT from interface. In this version it is not mechanically possible yet. We need to disconnect them from MPPT first.
* Remove PV Input and OUTPUT cables from MPPT.
* Remove all other cables from MPPT.
* Remove the interface bleding.
* Remove PV Input and OUTPUT sockets with cables. Now it is possible to do.
* Put away the interface blending.

### Remove MPPT
* Remove screws which hold the MPPT.
* Put away MPPT.

### Remove BMS
* Remove screws which hold BMS at the battery case.
* Put away BMS.

### Remove remaining side blendings
* Remove remaining side blending and put them away.

Now you can easier access the batteries.

### Remove batteries
* Determine the in wich order you need to remove the batteries. We work from **main -** -- this is the first battery -- to **main +** -- this is the last battery.
* Carefully remove a screw, an electric connector, and a washer from one side of a battery block.
* Carefully remove a screw, an electric connector, and a washer from the other side of the battery.
* Put away the battery.
* Repeat it for all the remaining batteries.

### Dissassemble frame
* Lay the frame on a side. This is the side with the largest area.
* Remove four upper screws.
Before remove the frame, pay attention to the nuts in the frame. They can fall down after the next step.
* Put away the frame.
* Remove four screws which connects the remaining frame with the small aluminum profiles.

We have now two frames and for short aluminiums profiles.

* Remove screws throw the plastic corners of the both frames.
* Remove the plastic corners.

