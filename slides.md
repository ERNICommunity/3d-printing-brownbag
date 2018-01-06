# 3D Printing

* In general 
* ... and with our Prusa i3 MK2

---

## 3D printers 

Note: 3D printers comes in different shapes ...

----

### Fused filament fabrication (FFF)
<!-- .slide: data-background="./Schematic_representation_of_Fused_Filament_Fabrication_01.png" -->

![FFF](fff.png)


---

## RepRap and big idea behind it

---

## Plastics

----

### ABS

----

### PLA

---

## From Idea to Thing

---

### 3D Modelling
Creating a model from scratch

----

#### 3D Builder
* Simple yet pretty powerful
* Part of Windows 10
* Can import and export _STL_, 3MF and other popular formats
* Can send model directly to a printer (or a 3D printing service)

----

#### Blender
* Free and open source 3D creative suite
* __Modelling__, rigging, animation etc.
* Very powerful, but with steep learning curve
* For 3D printing, best used for modelling and mesh manipulation

----

#### OpenSCAD
* CAD (computer-aided design) tool
* Great for designing very precise models for stuff like machine parts
* Not an interactive modeller - it uses a scripting language to describe the models
* Exports _STL_

---

### Slicing
Making a model printable

----

#### The Idea
* 3D Printers don't understand 3D models
* They require specific instructions on where to move the extruder and how much filament to extrude
* Slicing is the process that takes a 3D model and outputs a _GCode_ that can be printed

----

#### Slic3r
TODO

----

#### Ultimaker Cura
* Originally used for Ultimaker printers
* Has presets for a wide variety of 3D printers, including Prusa
* More intuitive UI compared to Slic3r
* Can set all the main and most of the detailed print options
* For Prusa-specific settings (such as Linear Advance) it's best to use Slic3r

---

### Data formats

----

#### STL
* Origin in "stereolithography"
* Describes only the surface of a 3D object
* No color, no material, no size, no units
* Basically just a set of polygons (also called _mesh_)
* Has ASCII and binary format
----

#### GCode
* AKA a printer program (more exactly it's a numerical control programming language)
* A sequence of machine-readable instructions for the printer
 - Homing, temperature control, calibration
 - Extruder movement, filament extrusion/retraction etc.

---

## Prusa i3 MK2

* Construction
* Firmware 
* Calibration (magic)
* Electronics

---

## Next steps with your prints

---

## Delete me (later)


> Best quote ever.

Note: speaker notes FTW!
