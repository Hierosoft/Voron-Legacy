# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).


## 2025-07-24
### Added
- y axis rod alignment tool [by deleted user on Discord]
- "X carriage for Stealthburner with CW2 for VL" by Ibbanez VL.029 on Discord.


## 2025-07-05
### Added
(Poikilos)
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
