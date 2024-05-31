# Dremel3D

This repo contains GCode for various settings of the Dremel3D DigiLabs printer. I've tweaked some of the settings so it applies to Dremel3D printers.

Starting GCode to print a test print line (from Cura):
```
G28 ; home X, Y and Z axis end-stops
G0 Z50.00 F400 ; Raise the bed
G92 E0 ; zero the extruded length
G1 F200 E3 ; Extrude 3mm of filament
G92 E0 ; zero the extruded length
M132 X Y Z A ; Recall home offsets
M907 X100 Y100 Z50 A100
G0 X-20.0 Y-50.0 Z0.3 F5000.0 ; Move to print test line
G1 X20.0 Y-50.0 F1500.0 E15 ; Draw the print test line
M132 X Y Z A ; Recall home offsets
```
