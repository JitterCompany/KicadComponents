# KicadComponents

Custom KiCAD component libraries by Jitter

## How to Install

### Schematic library

To install the schematic library, open the *Symbol Library Editor*. Then go to *preferences* -> *manage symbol libraries* and add an entry with the nickname "Jitter_Components".

### Footprint library

 To install the footprint libraries, open the *Footprint Editor*. Then go to *preferences* -> *manage footprint libraries* and add these entries:
 * *Jitter_Footprints*
 * *Jitter_Logos*
 
 ### 3D footprints
 
 Open the *Footprint Editor*. Go to *Preferences*, *configure paths*.
 Under *3D Search Paths*, add an alias *'jitter'*. The path should be the absolute path to the *3D* folder in this repository.
 
 All footprints pointing to a 3d file in te format *jitter:<my3dshape.step>* should now resolve correctly.
