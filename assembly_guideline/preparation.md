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

## Assembly
### Assembly frame box
Note: square nuts are not symmetric. When inserting them into T-Slot, keep the upper part outside. See picture [...] to determine the upper side of the nuts.

Create large squre frames first.

* Put larger profiles on the table and put plastic corners in the corners. Check orientation of the profiles. The holes on the side of the upper and the lower profile must be up.
* Insert all necessary square nuts in the T-slots.

 Hint: Use a bolt to push a square nut into a slot.

* Control the placement of corners, screws and squre nuts.
Start with the bottom part.
* Connect a corner to the bottom.
* Connect a side part to the bottom.
* Connect another corner to the bottom.
* Connect another side to the bottom.
* Connect remaining corners and the upper part.
* Connect small T-profiles to a big square frame. The holes on the side of the large frame must be later outside of the box.
* Insert nuts into short profiles. Two nuts into every short profiles on the top of the future box. Four nuts into every short profile on the bottom of the future box.

### Add bottom
* Add the bottom blending.

### Add batteries
* Mark the batteries with numbers *1*, *2*, *3*, and *4*.
* Put batteries into the battery case.
* Isolate main **+** and main **-** of the batteries. (Is it important to have main "+" or "-" on particular side of the battery block?")
Now carrefully connect batteries one by one, from *4* to *1*.
* Put connector between *4* and *3*.
* Put a washer on the connector on the side *4*.
* Put thin cable with tag *4* on the washer
* Put another washer on the connector of the thin cable. (Too many washers, check it again).
* Put a bolt throw connector, washers and thin cable and  tighten it. (bots or screws?).
* Put a washer on connector on side *3*.
* Put a bolt throw the washer and the connector and tighten it.
* Connect in the simmilar way batteries *3* with *2* and *2* with *1*.
* Do **not** remove isolation from main **+** and main **-** yet.

### Assembly interface bleding
The interface blending is the blending with sockets.
* Put sockets with cables into the blending
* Mount the interface bleding to the frame

### Connect BMS
* Solder cablers to the on/off-switch.
* Mount blue thick cables and USB+ to *PWR-* of BMS.
* Mount red thick cables and USB- to *PWR+* of BMS.
* Connect two blue cables (- or +?) to two DC out sockets.
* Connect two red cables to two DC out sockets.
* Connect two thin cables from on/off-switch to BMS.

### Connect to MPPT
* Connect all cable ends without blade connectors to MPPT.
* Check that these cable are well mounted.

### Connect battery block
(In this part BAT- and BAT+ seems to be confused.I need resolve it.)
* Remove isolation from **main -**.
* Connect two cables to **main -**.
* Connect thick blue cable to *BAT-* on BMS.
* Connect two cables to **main -**
* Connect balancing to *BAT-* on BMS. (Is this correct?)
(Must the on/off switch must be off before add the fuse? How one can see it?)
* Add fuse.
* Check the voltage (where?): It must be around 12.8 V.
* Switch off the on/off switch.
* Check the voltages. It must be falling until 0. The voltage does not drop imidiatelly to 0, because there is remaining electric charge in the capacitors.
* Swich on.
* Check Voltage between *POW+* and *POW-*. It must be about 12.8V.
* Remove the fuse. (I missted this step in my notes. Is it correct here?).

### Connect Raspberry
* Connect  an internet cable to Raspberry
* Connect the internet cable to BMS.
* Connect an internet cable to CAN socket on the blending.
* Connect the other end of the cable to BMS.
* Mount the Raspbery with two-side tape to the box.

### Add back blending
(Better do it before interface blending because the inteface blending is not flat.)
* Put SolarBox on the interface.
* Position square nuts. They must have the same position as the holes of the blending.
* Put blending on the frame.
* Insert bolts through the blending into the square nuts. Tighten the bolts.

### Mount side blending
* Put the SolarBox on the side.
* Position the squre nuts.
* Put the blending on the frame.
* Insert bolts through the blending into the square  nuts. Tighten the bolts.

### Mount to blending with handles.
* Put the SolarBox on the bottom.
* Position squre nuts for the top blending.
* Put top blending.
* Put handles on the top blending.
* Insert **longer** bolts through the handles, the blending and squre nuts. Use normal bolts for other parts of the blending.
* Tighten the blending.

### Mount last side blending
* Check once more if all the connection are good.
* Insert the fuse.
* Put the SolarBox on the side.
* Position the square nuts.
* Add the blending.
* Tighten the bolts.
