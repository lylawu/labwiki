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
**Build Volumn:** 25×21×21 cm (9.84"×8.3"×8.3")
**Nozzle:** 0.4mm default, other diameters supported
**Filament used:** PLA, PETG, ASA, ABS, PC (Polycarbonate), CPE, PVA/BVOH, PVB, HIPS, PP (Polypropylene), Flex, nGen, Nylon, Carbon filled, Woodfill and other filled materials.
**Filament diameters:** 1.75 mm
**Printer dimensions:** ( without spool) 7 kg, 500×550×400 mm; 19.6×21.6×15.7 in (X×Y×Z)
**Max travel speed:** 200+ mm/s
**Max heatbed temperature:**  120 °C / 248 °F 
**Max nozzle temperature:** 300 °C / 572 °F
**Print Surface:** Removable magnetic steel sheets(*) with different surface finishes, heatbed with cold corners compensation
**Power consumption:** PLA settings: 80W / ABS settings: 120W

Official Handbook: [Here](https://cdn.prusa3d.com/downloads/manual/prusa3d_manual_mk3s_en.pdf#_ga=2.238010112.1277322509.1687747893-905613141.1686940624)

## How to prepare a printable file in Rhino
1. Check for errors: Make sure the model fits within the Prusa i3’s build volume. Use Rhino’s built-in tools to check for manifold issues, close holes or broken surfaces, open edges, duplicated surfaces. 
2. Scale: Make sure your object is properly scaled. Prusa i3 usually reads dimensions in millimeters.
3. Orientation: Position your object in a way that minimizes the need for support structures and maximizes print quality.
4. Wall Thickness: Ensure that your model has adequate wall thickness to support the structure during and after printing.
5. Join and Unify Normals: If your model consists of multiple parts, join them together into a single watertight mesh. Make sure the normals are unified.
6. Test for Printability: Use Rhino’s Check command to evaluate the geometry for any flaws or issues that could affect print quality.
7. Export: Go to File > Export Selected, and choose the STL (.stl) format from the options. This is a commonly used file format for 3D printing.
8. STL Export Options: In the dialog that appears, you'll usually want to select “Binary” for smaller file sizes, and ensure that your units are set to millimeters.
9. Mesh Settings: Depending on the quality you desire, you might have to tweak the mesh settings. Higher mesh densities often result in higher quality prints but increase file size.
10. Save: Name your file and choose a location to save it.


## Setting up 3D-printing software on your computer (PrusaSlicer)
1. Download and install [PrusaSlicer](https://www.prusa3d.com/page/prusaslicer_424/)
   
2. Once PrusaSlicer is installed, the configuration menu may pop up. If it doesn't, manually open it by going to Configuration --> Configuration Wizard in the top bar.
   
![Prusa](/assets/images/prusa0.png)

3. Go to Prusa FFF and select the Original Prusa I3 MK3 & MKS3+. Then, press finish on the bottom left.
![Prusa](/assets/images/prusa1.gif)

## Step-By-Step Printing Guide
- Here is a [PrusaSlicer Beginner Tutorial](https://www.youtube.com/watch?v=_kIqMPNQNSw) that will teach you the basics. The following bullet points will also serve as a guide to printing your first 3D model.
  
1. Create a 3D model or find one online. You can find some on [thingiverse.com](www.thingiverse.com). We will be printing the [Calibration Cube](https://www.thingiverse.com/thing:1278865).
Supported file types are: STL, STEP, 3MF, OBJ, and AMF.

![Calibration Cube](/assets/images/CalibrationCube.jpg)


3. Open the file in PrusaSlicer. If your file is in a zip, you must unzip it to access it. You can either drag the file from your downloads to PrusaSlicer, use CTRL + I, or import it by going to File --> Import --> Import STL/3MF/STEP/OBJ/AMF/PRUSA
   
<img src="https://github.com/PKMN-Python/labwiki/blob/main/assets/images/prusa4.gif?raw=true" data-canonical-src="https://github.com/PKMN-Python/labwiki/blob/main/assets/images/prusa4.gif?raw=true" width="720" height="400" />

4. Your model should now be in PrusaSlicer. Make sure the filament selected is PETG (unless you are using a different filament). You may want to edit your model's position or change some print settings, such as the nozzle size, quality, and amount of infill. If your model is tall and overhangs, it is recommended that you go to Print Settings --> Support Material --> and toggle Generate Support Material on. For this demonstration, we will be using the default settings.
   
![Prusa](/assets/images/prusa5.gif)

5. Once your model and print settings are finalized, press Slice Now at the bottom left of the screen. You should be able to see the supports and check how the infill looks in your model. You can also see the estimated print time.
   
6. Plug in the SD card from the printer into your computer. Export the file to your SD Card by either doing CTRL + U or going to File --> Export --> Export G-Code to SD Card. It is recommended that you rename the file and make it clear. Now, eject your SD card.

![Prusa](/assets/images/Prusa6.gif)

7. You are now ready to print! Bring your SD Card and plug it into the printer (on the left side of the control screen). On the screen, scroll down to your print by rotating the control knob. Press the knob to select. Press again to bypass any firmware notices. The bed will now heat up, and the print should start in a few minutes. You should see the estimated print time on the right.

![Prusa](/assets/images/Prusa7.gif)

8. Once your print has finished, wait until the bed has cooled down to room temperature, as this makes it easier for the print to come off. Use a spatula to take out the print or remove the bed and slightly flex it to separate the print from the bed.
   
9. If your print has supports, you can remove them with tweezers.


## Troubleshooting + [Calibration Guide](https://help.prusa3d.com/category/calibration_199) 
- If the filament is not sticking to the printer bed, remove the sheet and clean it with rubbing alcohol.
- If you switch out a steel sheet for another type, make sure to re-calibrate the bed.
- If you notice the nozzle is touching too close or too far from the bed when printing, you can adjust the height of the nozzle by changing the z-axis in the printer's configuration or live adjust the z-axis while printing.

![Prusa](/assets/images/prusaIssue1.png)
![Prusa](/assets/images/prusaIssue2.png)
![Prusa](/assets/images/prusaIssue3.png)

## How to load and unload filament on Prusa i3?
[Prusa i3 MK2 Quick Tip 005: Loading Filament - Bing video](https://www.bing.com/videos/search?q=Prusa+i3+loading+filament&view=detail&mid=CDED7A958C79FFCB8984CDED7A958C79FFCB8984&FORM=VIRE)
How To Load Filament in Prusa i3 (https://help.prusa3d.com/article/manual-temperature-calibration_2232)


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


# Postproduction

{: .fs-6 .fw-300 }
