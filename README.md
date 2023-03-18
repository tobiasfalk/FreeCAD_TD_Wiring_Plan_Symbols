# FreeCAD_TD_Wiring_Plan_Symbols
 this repo is a start for a collection of symbols for a Wiring plan WB in FreeCAD

## Structure
The symbols are done as a svg with some extra tags:

The description tag is for general information about the symbol with:
* name for the name of the symbol, should also be the file name
* designator for the symbol designator, like "L1", "L2", "K1", "K2", ..
* description for a description about the symbol
* origin for putting the origin of the model, where it comes from/who it created
* name-alias for synonyms and translations, makes searching for something easier
* symbol-alias for referencing a other symbol that displays the same thing but in a different form, like there is a US and European version for resistors
* 3d-model-name for linking the symbol to a FreeCAD model/file, this would allow future features where this WB interacts with the 3D space


The pin tag, this tag has the following options:

* pin is the pin number, could also be "A1", "B2" and so on, in some cases you want those numbers also be displayed nearr the pin but I would do this with svg tex
* x and y for the location
* type for differentiate between different types of pins, for example a electrical, fiber or hydraulic connection, with this itt would be posable to prevent th connection between a hydraulic and a fiber connection :D
* e-type this is a Idea for not only saying that general type but also how the pin interacts with other pins, posable value options would be "passive" for pins that are passive and do not much or "input" for pins that only take signals in, there could than also be a h-type for hydrolics and so on, if done correctly a rule check could be implemented/done where FeeCAD checks that you do not connect two input to each other without a output on the line
* 3d-model-ref this is for location the pin in the 3D space, I only say toponaming problem
* connection-type this is for defining how this pin is represented in the 3D space, is it a "screw terminal" or a other connection type, for fibers the connector name("LC") and hydraulics the thread pitch(?)

By the text tag the option " always-horizontal="true" " was added, this is for situations like the Ampmeter ore the Motor, there a letter is in the center and I personally think that should always be in a readable direction, so if the symbol is rotated this text should not be rotated.

## Size
The symbols are made for a 5mm grid and a line width of .35mm

## References
https://www.nrc.gov/docs/ML1025/ML102530301.pdf
https://www.theiet.org/media/4173/units-and-symbols.pdf
https://www.reconelectrical.co.uk/image/data/pdfs/Electrical%20Symbols%20Guide.pdf

https://www.electronics-tutorials.ws/resources/basic-schematic-symbols.html
https://www.electronicshub.org/symbols/

KiCAD Symbol Library