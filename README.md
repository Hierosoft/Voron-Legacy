# VORON Legacy

![Image of Voron Legacy](https://vorondesign.com/images/voron_legacy_bg.jpg)

The official release of the Voron Legacy 3d printer. You can find the BOM and any other relevant information at the [Voron Design]( http://vorondesign.com/voron_legacy) website.

![Voron Logo](https://vorondesign.com/images/voron_design_logo.png)

## Sourcing Guide
- See "VORON 1.6.2" at [sourcing guides](https://vorondesign.com/sourcing_guide?model=VL) page (1.6.2 is same as Legacy according to nemgrea)


## Assembly
- Voron Legacy [Brief assembly Guide](https://forum.vorondesign.com/threads/brief-assembly-guide.176/) by Sanity Agathion, a Voron forum admininstrator.
- Unofficial assembly video series: [Voron Legacy](https://www.youtube.com/playlist?list=PLm2OH_myqt7a_PT0lViufZZBrC22PzAQH) by [Fugatech 3D Printing](https://www.youtube.com/@Fugatech3DPrinting) on YouTube
  - Uses drop-in not slide-in T-nuts, so if using slide-in ones, take care to insert them before locking them out via assembly. See unofficial assembly manual below for image and description of where to insert them.
- [Voron Legacy Unofficial Manual by Poikilos](https://docs.google.com/document/d/1mR3VX70ok1uY0DY2WcfInHhRfALJT7SdbVQVug27Xh0/edit?usp=sharing)
  (WIP)

### Known issues
(Differences mentioned are from actual measurements of motors, and making belts centered on gearheads' teeth. Belts are in blend file in Poikilos' Voron Legacy folder on Google Drive)
- (CAD folder) Make motor shaft of A & B motors 0.152 mm longer so they are 24mm from the screw surface like motors in the 1.6.2 BOM
- Move A (right) gearhead (T20 pulley) down by 2.35 so it is 3.45 less than end of motor shaft
- Move B (left) gearhead (T20 pulley) up by 0.10217 so it sticks out 1.25mm more than end of motor shaft


## Contributors
- [deleted user] via Discord
  - "jig for aligning the Y axis rods with the frame" [2022-08-09](https://discord.com/channels/460117602945990666/791364306276450337/1006420060069441627)
    - y_axis_rod_alignment_jig_x4.stl (originally named legacy_tool.stl)
      - (4) are required as cited on [Brief assembly guide](https://forum.vorondesign.com/threads/brief-assembly-guide.176/)
- Ibbanez VL.029 via Discord
  - "X carriage for Stealthburner with CW2 for VL" [2022-08-24](https://discord.com/channels/460117602945990666/791364306276450337/1012131175113949204) as cited on [Brief assembly guide](https://forum.vorondesign.com/threads/brief-assembly-guide.176/)
    - X-VL_left.stl
    - X-VL_right.stl
- Poikilos
  - Alternate leadscrew block for anti-backlash POM nut (2 shank holes, spaced further apart).
    - Fits ["Ender 3 V2 Z axis T8 POM Anti Backlash Spring Loaded Nut Elimination Gap Compatible with Voron 2.4 Ender3 pro 3D Printer 8mm Acme Threaded Rod"](https://www.amazon.com/dp/B088FPNVVF?ref_=ppx_hzsearch_conn_dt_b_fed_asin_title_1) from POLISI3D Store on Amazon.
      - Be aware, these are consumable (will eventually tear apart and lose the threads)! Regular brass ones are recommended in the sourcing guide.
  - Alternate 206mm bed screw spacing parts (for reusing bed from A8 clone such as A3S)
    - 206mm on y: STLs/Tools/alternate_bed_screw_y_spacing_206mm/z_component_alignment_jig-206mm_bed_screw_spacing_A3S.stl
    - 206mm on x: STLs/Z Axis/Bed Carriages/alternate_bed_screw_x_spacing_206mm/
  - Blend file with the above, blind joints, and taller to use prefabricated Voron 2.4 frame:
    [Poikilos' Voron Legacy Folder](https://drive.google.com/drive/folders/1cWyBRrxuDkORSMTYZdLJZKc8Kg_imgok?usp=sharing) on Google Drive (too large for git except with LFS).
    - [Generated BOM](https://drive.google.com/file/d/1eSlRInvPNuWncBucrcRtuzRmA0uxTkT_/view?usp=sharing), reusing a prefabricated Voron 2.4 frame size
      - No 320 motors exist though, so use a regular stepper motor, flexible coupling (See unofficial sourcing guide below), and ~300mm lead screws such from A8 clone such as A3S.
    - Unofficial sourcing guide by Poikilos: [https://docs.google.com/spreadsheets/d/1isZgUZrGUJIj4jxUcvnwxng9hJ9_i8DxyWfmX4hRLIU/edit?gid=2118759969#gid=2118759969](Building VORON Legacy but with V2.4 Frame and salvaged A8 clone)
      - based on "VORON 1.6.2" at [sourcing guides](https://vorondesign.com/sourcing_guide?model=VL) (1.6.2 is same as Legacy according to nemgrea)
