# Configuring KiCAD Libraries 
will be finished soon™

KiCAD handles library parts a bit differently than other layout tools:

`schematic symbols aren't married to layout footprints in KiCAD!!!`

they *can* be correlated, but it isn't a requirement until invoking the netlist during the transition from schematic capture to layout. The [Digi-Key github](https://github.com/digikey/digikey-kicad-library) does a nice job of introducing the concept.

Luckily, after accepting the above, KiCAD library managment is fairly painless.

## Initializing the Digi-Key libraries
Digi-Key maintains a free KiCAD parts library! The library is far from comprehensive, but it's a nice start to building a respectible parts list to choose from. 
1. Start by copying the Digi-Key repo locally: [https://github.com/digikey/digikey-kicad-library](https://github.com/digikey/digikey-kicad-library). (green "clone or download" button, then download zip)
2. 
