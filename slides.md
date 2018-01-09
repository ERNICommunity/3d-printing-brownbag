# 3D Printing

* In general 
* ... and with our Prusa i3 MK2

by Marek Linka and Jakub Šturc
---

## Different types of 3D printers 

----

### Extrusion

![FFF](fff.png) <!-- .element height="50%" width="50%" -->

Scopigno R., Cignoni P., Pietroni N., Callieri M., Dellepiane M. (2017). "Digital Fabrication Techniques for Cultural Heritage: A Survey". Computer Graphics Forum 36 (1): 6–21. DOI:10.1111/cgf.12781.<!-- .element style="font-size:0.15em; color: grey" -->

----

### Light polymerized

![SLA](sla.png) <!-- .element height="30%" width="30%" -->

Scopigno R., Cignoni P., Pietroni N., Callieri M., Dellepiane M. (2017). "Digital Fabrication Techniques for Cultural Heritage: A Survey". Computer Graphics Forum 36 (1): 6–21. DOI:10.1111/cgf.12781.<!-- .element style="font-size:0.15em; color: grey" -->

----

### Powder Bed

![3DP](3dp.png) <!-- .element height="50%" width="50%" -->

Scopigno R., Cignoni P., Pietroni N., Callieri M., Dellepiane M. (2017). "Digital Fabrication Techniques for Cultural Heritage: A Survey". Computer Graphics Forum 36 (1): 6–21. DOI:10.1111/cgf.12781.<!-- .element style="font-size:0.15em; color: grey" -->

----

### Laminated

![LOM](lom.png) <!-- .element height="50%" width="50%" -->

By LaurensvanLieshout (Own work) [CC BY-SA 3.0], via Wikimedia Commons <!-- .element style="font-size:0.15em; color: grey" -->

---

## RepRap

<!-- .slide: data-background-image="oshw.png" data-background-size="50%" -->

----

<!-- .slide: data-background-image="oshw.png" data-background-size="50%" -->
* RepRap is humanity's first general-purpose self-replicating manufacturing machine.
* RepRap is short for replicating rapid prototyper.
* The RepRap project started in England in 2005 as a University of Bath by Dr Adrian Bowyer.

----

<!-- .slide: data-background-image="oshw.png" data-background-size="50%" -->
### The first replication - 2007

![The first replication](First_replication.jpg)

----

<!-- .slide: data-background-image="oshw.png" data-background-size="50%" -->
### RepRap Mendel - 2009
![Mendel](mendel.jpg)

----

<!-- .slide: data-background-image="oshw.png" data-background-size="50%" -->
### Prusa Mendel - 2010
![Prusa Mendel](prusa-mendel.jpg) <!-- .element height="50%" width="50%" -->

----
 
<!-- .slide: data-background-image="oshw.png" data-background-size="50%" -->
### Jellyfish - 2012
![eof](jellyfish-eof.jpg)

---

## Plastics

----

### Polylactic acid 

<!-- .slide: data-background-image="pla.png" data-background-size="50%" -->

* Made from corn, sugar cane or any starchy vegetable
* Biodegradable and can be fully recycled
* Somethimes used in body implants

----

### Polylactic acid

<!-- .slide: data-background-image="pla.png" data-background-size="50%" -->

* Easy to print with
* Does not smell or smell like candy
* Almost does not warp
* Print temperature: 190°C – 230°C 
* Bed temperature: 20°C – 60°C
* Hard but brittle

----

### Acrylonitrile butadiene styrene 

<!-- .slide: data-background-image="abs.png" data-background-size="80%" -->

* Bicycle helmets and Lego is made from ABS
* Derived from natural gas or crude oil
* Sometimes used in tatoo inks
* At 400 °C decompose to carcinogenic stuff
* During 3D printing may produce ultra fine particles

----

### Acrylonitrile butadiene styrene 

<!-- .slide: data-background-image="abs.png" data-background-size="80%" -->

* Slightly more difficult to print with
* Smells (still acceptable)
* Tendency to warp during cooldown
* High temperature tolerance −20 to 80 °C 
* Print temperature: 220°C – 250°C 
* Bed temperature: 80°C – 110°C
* Hard and slightly flexible
* Does not like long-term sun (UV) exposure

----

### Other Plastics

* PETG 
* Nylon
* Solvable (HIPS, PVA)
* Flexible (TPE, TPU, TPC flexible)
* Wood (PLA with wooden fibers)
* Metalic (PLA/ABS with metal powder)
* Glowing (PLA/ABS with glowing stuff)
* Magnetic, Conductive (PLA/ABS with other stuff)
* ...

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
* For Prusa-specific settings (such as Linear Advance) it's best to use Slic3r and/or PrusaControl
* Latest version (3.1) is bugged, recommended to use 3.0.4

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

----

### Construction
* A combination of metal and plastic parts
* Plastic parts are all 3D printed
 - In accordance with the idea of self-replication
* Metal parts need to be purchased
* Most of the components can be exchanged or modified

----

### Firmware
* The brain of the printer
* Open source (hosted on github)
* Open to pull requests
* Periodic updates
 - Last version: linear advance feature
* Allows for nifty features such as autocalibration and bed skew correction

----

### Calibration
* This is where the magic happens
* You mainly want to get the first layer to stick to the bed
* Experimental process, dependent on many parameters
 - Bed level skew
 - Filament used (not even two PLA filaments are the same)
 - Distance between bed and extruder
 - Extruder and bed temperature etc.

----

### Making it work
* Each print will be different
* Different slicers have different outcomes
* If the first layer doesn't stick, experimentation is required
 - Lower the extruder
 - Increase filament flow
 - Change temperatures etc.
* there is no RIGHT answer here
* Just try it and see

---

## Next steps with your prints
1. Buy printer
2. Download model
3. ???
4. PROFIT!

----

### When YOU want to print stuff
* Create or find a model
* Pick a filament (PLA/ABS, color)
* Think about how you want to slice it (with supports, with adhesion plate etc.)
* Slice it or ask how to do it
* Be ready to stand watch as the first layer sets
* Keep an eye on the print

---

<!-- .slide: data-background-image="fail.jpg" -->
### Everything will go wrong
* 3D printing is more alchemy than chemistry
* Stuff that can go wrong will go wrong
* Be prepared for bad prints
* Get familiar with settings and options of both slicer and printer
* Experiment - trial and error will get you far

----

> __Failure is ALWAYS an option.__

> -- _Adam Savage_

---

## Thank you
