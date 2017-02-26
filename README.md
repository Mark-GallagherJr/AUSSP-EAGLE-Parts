# AUSSP-EAGLE-Parts
Contains parts for EAGLE not included in the default libraries.
These parts were made in EAGLE 6, but should be compatible with current versions of EAGLE. They will be missing the 3D attributes used by the 3D renderer in EAGLE 7 and above.

## Installation
The following procedures explain how to install these files into EAGLE:

1. Download this repo as a .zip
2. Extract the .zip into a folder called, for example, "AUSSP-custom-lbr"
3. Navigate to the folder: "EAGLE_INSTALL_DIR\lbr", where "EAGLE_INSTALL_DIR" is wherever you installed EAGLE
  * This is usually at the root of your drive, for example, "C:\EAGLE 8.0.2"
4. Move your folder, "AUSSP-custom-lbr" into EAGLE's lbr folder
5. Launch (or restart if already open) EAGLE
6. In the Control Panel, open the "Libraries" resource on the left and ensure your libaries appear
7. Expand your AUSSP custom libaries to see all of the libraries included
8. If the dot to the right of each of the library's name is gray, you need to enable these libraries:
  * Do this by clicking the dot so that it is now green. Repeat for all libraries in the list
9. Open a schematic and try to add a part (command: ADD, or shortcut: SHIFT+CTRL+A)
10. In the parts dialog, check to be sure your libraries are installed.
  * If not, you may need to go back to the schematic and go to "Library->Update all" in the menubar to refresh the library listings
  * If you still can't see them, then go to "Library->Use..." and select all of your custom libraries to use, then do an Update all

## Information on some of the libraries:

### AS2_AVIONICS_LOGOS.lbr
Contains logos used in the AS-2 days. Not really relevant for new projects, just nice for aesthetics.

### AS-2-Extras.lbr
Contains a lot of random parts made during the AS-2 days. About the only relevant component here is the "INA219" part (current sensors).

### AUSSP_Logo.lbr
Just a logo for AUSSP use. 

### AUSSP_sch_template.lbr
Use this for enclosing your schematics in a pretty, AUSSP-branded, box. This is what is currently in-use for all Avionics designs. 

### adafruit.lbr
A modified version of the Adafruit library available also on Github. In this version, I modified the capacitors so that they include a "tolerance" attribute.
