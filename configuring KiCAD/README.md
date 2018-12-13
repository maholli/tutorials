# Configuring KiCAD Libraries 
will be finished soon™

KiCAD handles library parts a bit differently than other layout tools:

`schematic symbols aren't married to layout footprints in KiCAD!!!`

they *can* be correlated, but it isn't a requirement until invoking the netlist during the transition from schematic capture to layout. The [Digi-Key github](https://github.com/digikey/digikey-kicad-library) does a nice job of introducing the concept.

Luckily, after accepting the above, KiCAD library managment is fairly painless.
## Adding OSH Park layout templates
1. Download the folders `oshpark-2lay` and `oshpark-4layer` (green "clone or download" button, then download zip)
2. Move the two folders to the following location on your machine, making sure to replace the portion with your respective install path: C:ReplaceThisWithYourKicadInstallPath\KiCad\share\kicad\template


## Initializing the Digi-Key libraries
Digi-Key maintains a free KiCAD parts library! The library is far from comprehensive, but it's a nice start to building a respectible parts list to choose from. 
1. Start by copying the Digi-Key repo locally: [https://github.com/digikey/digikey-kicad-library](https://github.com/digikey/digikey-kicad-library). (green "clone or download" button, then download zip)
2. 

## Useful Plugins
If you're using a nightly build of KiCAD (I've been using [kicad-r11831.c539d6e0b-x86_64](http://downloads.kicad-pcb.org/windows/nightly/) with good success), it will let you install external plugins for Pcbnew. Here are some repos w/ plugins I found useful:
* [https://github.com/easyw/kicad-action-plugins](https://github.com/easyw/kicad-action-plugins) super helpful for moving things between layers
* [https://github.com/openscopeproject/InteractiveHtmlBom](https://github.com/openscopeproject/InteractiveHtmlBom) beautiful HTML BOM generation tool. 

Make sure to move the plugins to the following directory on your machine: 
`C:ReplaceThisWithYourKicadInstallPath\KiCad\share\kicad\scripting\plugins`

For Mac that usually looks like...? `/Library/Application Support/kicad/scripting/plugins`
