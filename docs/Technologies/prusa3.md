---
layout: default
title: Prusa3
nav_exclude: true
has_children: false
permalink: /docs/technologies/prusa3
---

# PRUSA i3 MK3

## Location

Main lab, 4 printers

## Technical Details

FDM Desktop Fabrication  
**Model:** Original Prusa i3 MK3  
**Brand:** Prusa Research  
Heated build Chamber  
**Filament used:** PLA, PETG    

## Setting up 3D-printing software on your computer (PrusaSlicer)
1. Download and install [PrusaSlicer](https://www.prusa3d.com/page/prusaslicer_424/)
2. Once PrusaSlicer is installed, the configuration menu may pop up. If it doesn't, manually open it by going to Configuration --> Configuration Wizard in the top bar.
![image](https://github.com/PKMN-Python/labwiki/assets/34625211/e5923246-407e-47d7-8aff-6ffebcc22e57)
3. Go to Prusa FFF and select the Original Prusa I3 MK3. Then, press finish on the bottom left.
![image](https://github.com/PKMN-Python/labwiki/blob/main/assets/images/prusa1.gif?raw=true)

## Step-By-Step Printing Guide
- Here is a [PrusaSlicer Beginner Tutorial](https://www.youtube.com/watch?v=_kIqMPNQNSw) that will teach you the basics. The following bullet points will also serve as a guide to printing your first 3D model.
  
1. Create a 3D model or find one online. You can find some on [thingiverse.com](www.thingiverse.com). We will be printing the [Calibration Cube](https://www.thingiverse.com/thing:1278865).
Supported file types: STL, STEP, 3MF, OBJ, and AMF.

3. Open the file in PrusaSlicer. You can either drag the file, use CTRL + I, or import it by going to File --> Import --> Import STL/3MF/STEP/OBJ/AMF/PRUSA
   
![image](https://github.com/PKMN-Python/labwiki/blob/main/assets/images/Prusa5.gif?raw=true)

4. Your model should now be in PrusaSlicer. Make sure the filament selected is PETG (unless you are using a different filament). You may want to edit your model's position or change some print settings, such as the nozzle size, quality, and amount of infill. If your model is tall and overhangs, it is recommended that you go to Print Settings --> Support Material --> and toggle Generate Support Material on. For this demonstration, we will be using the default setting. 

5. Once your model and print settings are finalized, press Slice Now at the bottom left of the screen. You should be able to see the supports and check how the infill looks in your model.
6. Plug in the SD card from the printer into your computer. Export the fil to your SD Card by either doing CTRL + U or going to File --> Export --> Export G-Code to SD Card. Now, eject your SD card.

![image](https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExdGl5Mmx1eG82bTZ6MzhnczB3ZW9wNDJvaTdqcmxvZTZxaWg0cjNoZiZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/XgZjfdCHE1pMLILphx/giphy.gif)

7. You are now ready to print! Bring your SD Card and plug it into the printer (on the left side of the control screen). 

## Fixing Errors + [Calibration Guide](https://help.prusa3d.com/category/calibration_199) 
- If the filament is not sticking to the printer bed, remove the bed and clean it with rubbing alcohol.
  - Whenever you remove the printer bed and put it back on, make sure to recalibrate the bed.
- If you notice the nozzle is touching too close or too far from the bed when printing, you can adjust the height of the nozzle by changing the z-axis in the printer's configuration.

![image](https://github.com/PKMN-Python/labwiki/assets/34625211/8cff9ae6-3740-4bf4-9194-b3389c5f075f)
![image](https://github.com/PKMN-Python/labwiki/assets/34625211/886305d4-9bbb-4025-80a8-3c757af3b8c3)
![image](https://github.com/PKMN-Python/labwiki/assets/34625211/082b2986-806d-4a18-bec7-9f3137492818)



## Features

- Magnetic bed with swappable steel sheets:
  - For easy and quick 3D print removal.
    - 3 Types: smooth, textured and satin which do not require surface preparation (i.e., glue, tape)
  - The flexible steel sheets have a PEI powder coating.
  - The print bed can reach up to 100C.
- Optical filament sensor:
  - Enables automatic filament loading.
  - Lets the user know when the filament is running out and pauses the 3D print.
  - Detects filament jams and stops the 3D printing process.
- Power panic: if there is a power outage, the MK3 will go back to where it last left off when the power is back. This feature works without batteries.
- Sensing fans and Noctua: for more silence when 3D printing. Also, cooling from both sides of the extruder increases the 3D printer&#39;s overhang performance.
- New Y axis: gives the 3D printer a smoother look and a sturdier frame.
- Bondtech extruder: dual gears ensure a reliable grip on the filament to prevent filament from slipping. The extruder can reach up to 300C.

## Cura Profiles

[PETG ](link.to.profile.here)
[PLA ](link.to.profile.here)


## Slicing Information  

| Technical specifications      | Details               |
|:------------------------------|:----------------------|
| File Dormat                   | STL, AMF              |
| Print Volume                  | 250mm x 210mm x 210mm |
| Minimum Layer Resolution      | 0.05 mm (0.002 inch)  |
| Max Print Speed               | 200 mm/sec            |
| Nozzle Diameter               | 0.4mm                 |
| X/Y Axis                      | 0.01 mm/step          |
| Z Axis                        | 0.05 mm/step          |
| Filament Diameter             | 1.75 mm               |
| Hardware Dimensions           | 420 x 420 x 380 mm    |
| Connectivity                  | SD Card               |


# PETG recomended settings

| Technical specifications      | Details               |
|:------------------------------|:----------------------|
| Temperature                   | 225  C                |
| Bed Temperature               | 90   C                |
| Print surface                 | PEI                   |
| Suggested resolution          | 0.2 , 0.3 mm          |
| Fan Speed                     | 50%                   |
| Wall thickness                | 1.2mm (3 lines)       |

# PLA recomended settings

| Technical specifications      | Details               |
|:------------------------------|:----------------------|
| Temperature                   | 110  C                |
| Bed Temperature               | 65   C                |
| Print surface                 | PEI, Blue tape        |
| Suggested resolution          | 0.2 , 0.3 mm          |
| Fan Speed                     | 100%                  |
| Wall thickness                | 1.2mm (3 lines)       |




{: .fs-6 .fw-300 }
