# FreeCAD_TD_Wiring_Plan_Symbols
 this repo is a start for a collecttion of symbols for a Wiring plan WB in FreeCAD

## Structure
The symbols are done as a svg with some extra tags:

The description tag is for general information about the symbol with:
* name for the name of the symbol, should also be the file name
* designator for the symbol designator, like "L1", "L2", "K1", "K2", ..
* description for a descripion about the symbol
* origin for puting the origin of the model, where it comes from/who it created
* name-alias for synonyms and translations, makes searching for something easyer
* symbol-alias for referencing a other symbol that displays the same thing but in a different form, like there is a US and European version for resistors
* 3d-model-name for linking the symbol to a FreeCAD model/file, this would allow future fetures where this WB interacts with the 3D space


The pin tag, this tag has the folowing options:

* pin is the pin number, could also be "A1", "B2" and so on, in some cases you want those numbbers also be displayed nearr the pin but I would do this with svg tex
* x and y for the location
* type for diferentiate betwen diferent types of pins, for example a electricla, fiber or hydrolic connection, with this itt would be posible to prevent th connection betwen a hydraulic and a fiber connection :D
* e-type this is a Idea for not only saying that general type but also how the pin interacts with other pins, posible value options would be "passive" for pins that are passive and do not much or "input" for pins that only take signals in, ther could than also be a h-type for hydrolics and so on, if done correctly a rule check could be implemented/done where FeeCAD checks that you do not connect two input to each othe witthout a output on the line
* 3d-model-ref this is for location the pin in the 3D space, I only say toponaming problem
* connection-type this is for defing how this pin is representaed in the 3D space, is it a "screw terminal" or a othe connection type, for fibers the connector name("LC") and hydrolics the thrread pich(?)

## Size
The symbols are made for a 5mm grid and a line width of .35mm

## References
https://www.nrc.gov/docs/ML1025/ML102530301.pdf
https://www.theiet.org/media/4173/units-and-symbols.pdf
https://www.reconelectrical.co.uk/image/data/pdfs/Electrical%20Symbols%20Guide.pdf

https://www.electronics-tutorials.ws/resources/basic-schematic-symbols.html
https://www.electronicshub.org/symbols/