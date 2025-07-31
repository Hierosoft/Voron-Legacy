# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).


## 2025-07-27
### Fixed
- Named unnamed inductive_probe.


## 2025-07-27
(only to blend file in Poikilos' Voron Legacy Folder on Google Drive)
### Added
- Belts (blend file)
### Fixed
- Edit end of A & B motor shafts so they are 24mm from the screw surface like motors in the 1.6.2 BOM.
- Move A (right) gearhead (T20 pulley) down by 2.35 (blend file) so it is out 3.45 less than end of motor shaft
- Move B (left) gearhead (T20 pulley) up by 0.10217 (blend file) so it sticks out 1.25mm more than end of motor shaft
- Move entire scene by -76.8922,-135.07,360.175 mm so top surfaces of bottom bars is at 0 on z axis and outer edge is at 0,0 on x-y plane.
  - Then rotate 180 on world origin so that x and y move in the same direction as they would in firmware and slicer software.


## 2025-07-26
(Poikilos)
### Fixed
- Named more parts in FreeCAD file (and Poikilos' blend file in Google Drive link):
  `front_idler_*`, `bed_carriage_*`, `z_leadscrew_block_x2` `z_shaft_support_upper_*`, `*_drive_unit_*`, `z_shaft_support_lower_*_x2`, `z_motor_mount_*_x2*`, `bowden_adapter_*`, `[a]_bowden_cable_cover`, `blower_housing_rear`, `[a]_blower_housing_front`, `printhead_*_e3dv6`, `probe_retainer_bracket`, `[a]_belt_clip_x2`, `enclosure_cover`, `psu_stabilizer` (was misspelled "Stabalizer"), `xy_joint_*`, `y_bearing_retainer_front_x2`,
  - Helps find the STL you need. Example: identifying parts in (unofficial) documentation visually rather than using a file search.
- Suffix assemblies for parts above with **"_ASSEMBLED"** to avoid confusion on export where parts are fused into one mesh but must be printed separately (impossible to print if fused, but at least user is clued into that fact and knows to not export that. This is fixed in Poikilos' blend file.).
- Parts with ".R" or rear/front in name do not have to be exported more than once (filename is part before dot).


## 2025-07-26
(Poikilos)
### Fixed
- Rename misspelled files: (3) Z axis `*support*` files formerly `*suport*`.


## 2025-07-24
(Poikilos)
### Added
- y axis rod alignment tool [by deleted user on Discord]
- "X carriage for Stealthburner with CW2 for VL" by Ibbanez VL.029 on Discord.


## 2025-07-05
(Poikilos)
### Added
- Added Google Drive link to Blend file (since blend file is over 100MB, so it cannot be uploaded to GitHub except with LFS).
  - Converted .step file to .gltf using [CAD Assistant](https://www.opencascade.com/products/cad-assistant/) (Generates good normals so less geometry is required, according to mrpraline on blender.stackexchange.com [Oct 18, 2020](https://blender.stackexchange.com/a/199076/12998)
  - Converted .gltf file to .blend file using Blender 3.6.19.
    - The intermediate models were large (nearly as large as the blend file), so not committed.
- bed carriage for 206mm screw spacing (for reusing bed from A8 clone such as JGAURORA A3S)
  - stock screw spacing (x, y): 214.6, 150
  - reused A8 clone bed screw spacing: 206, 206
  - difference: 8.6, -56
  - Changed Y bed screw spacing from 150 to 206 (each outward toward front & back by 28 mm). Affects:
    - position of vertical rod mounts (See alternate z axis component alignment jig)
    - bed carriage uppers (use longer bar so mounts can be spaced more)
      - requires (2) 186mm 2020 extrusions rather than the stock 130.
  - Changed X bed screw spacing from 214.6 to 206 (each inward by 4.3 mm)
    - Moved hole & added more material (See alternate bed carriage uppers)
  - Changed PCB heater size to 213.5 x 213.5 (reduced by 7.55 mm on each side).
    - This is just to help mods/changes account for heating elements.

### Changed
(Poikilos)
- Make blind joint version blend file
  - Scaled to match a prefabricated VORON V2.4 frame kit.
  - Increased length of vertical HFSB5-20 from 370 to 430
    - increase by 60
    - move down by 20
  - Increase length of vertical linear rods by 340 (320 + 20)
  - Rotate z 90 so X and Y of printer line up with world
  - Move frame to center it on the world origin.
