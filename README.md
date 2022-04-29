# MIB2 backlight Menu
Research about ambient illumination controls in MIB2 infotainment system.

Based on my findings in VW Golf MK7 with MST2 system.

![VW Golf MK7 facelift Backlight menu with 5 zones](https://github.com/mrfixpl/mib2-backlight-menu/blob/main/pictures/VW-Golf-MK7-facelift_5-zones.png)

## `0x5F` MIB2 coding and adaptation
### Enable interior illumination controls
`0x5F` → `adaptation` → `Car_Function_Adaptations_Gen2`:
* → `menu_display_ambient_illumination` → `active`
* → `menu_display_ambient_illumination_over_threshold_high` → `active`

### Enable MIB `0x5F` communication with BCM `0x09`
`0x5F` → `adaptation` → `Car_Function_Adaptations_Gen2`:
* → `Interieur light 0x08` → `activated`
* → `Interieur light 0x08 msg bus` → `comfort data bus`

### Review vehicle variant coding
`0x5F` → `Long Coding` → Bytes `0-2`

More details in `.gcc modifications` section.

## `0x09` BCM coding and adaptation

## `.gcc` modifications
*coming soon...*

## GUI modifications
*coming soon...*

## Credits, Reference, Tools
* Cuzoe research: https://www.golfmk7.com/forums/index.php?threads/rgb-ambient-lighting-hopes-dreams-pre-facelift-mk7.392316/
* MIB STD2 Toolbox: https://github.com/olli991/mib-std2-pq-zr-toolbox
* OBDeleven diagnostic interface (ref link): http://obdeleven.com/?src=link&ref=Zy245Iacqc6bMTHh
