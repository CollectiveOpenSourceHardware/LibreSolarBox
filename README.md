# Libre Solar Box
This Open Hardware project is about the development of a solar box.
We want to provide a compact, mobile and modular electric power generator. An alternative to the diesel generator.
The power specifications are chosen to supply a mini house, a boat, a caravan, or any other off-grid devices like a music station on an open-air.

The aim is that everybody is possible to rebuild the solar box at home or at his/her favourite fablab.

![Layout](/LibreSolarBox_Layout.png)

----------------------
## current system layout, V0.1
The current Libre Solar Box system contains following specs and modules:
### specs:
- V_input_max = 55V
- P_input_max = 300Wp
- C_batteries = 920 Wh
- V_dc_out = 12V
- P_dc_out = 300W, theoretically 600W -> not tested
- (V_ac_out = 230V, 50Hz) optional
- (P_ac_out = 250W) optional -> depend on inverter

### modules:
- **electric**: [Libre Solar](http://libre.solar/) (MPPT+BMS), Inverter (Victron), ESP/Rasbperry, Fuse
- **Batteries**: LiFePO4 (Calb), 72Ah, 3,2V, 230,5Wh - 4x -> 12,8V, 920Wh
- **Housing/Frame**: [UniProKit](https://wiki.opensourceecology.de/Upklib), with corner elements for blending; wood plates for mounting electric parts and batteries
- **Interface**: Solarinput (MC4), DC-output (car plug), AC-output (schuko, integrated in inverter), main switch

### visualization:
- [Open Energy Monitor](https://openenergymonitor.org/) via CAN to ESP (Server ext.)/Rasbperry (Server int.)
- browser based visualization -> access via LAN/WLAN

