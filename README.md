# KicadComponents

Custom KiCAD component libraries by Jitter

## How to Install

### Schematic libraries

To install the schematic library, open the *Symbol Library Editor*. Then go to *preferences* -> *manage symbol libraries* and add an entry for each library:

* *Jitter_Components*
* *Jitter_IC*

**NB: for Kicad 6, make sure to select the `.kicad_sym` libraries**. The .lib are deprecated and for Kicad5.x only.

### Footprint libraries

 To install the footprint libraries, open the *Footprint Editor*. Then go to *preferences* -> *manage footprint libraries* and add these entries:
 * *Jitter_Footprints*
 * *Jitter_Logos*
 * *Jitter_IC*
 * *Jitter_Passives*
 * *Jitter_Connectors*

 ### 3D footprints

 Open the *Footprint Editor*. Go to *Preferences*, *configure paths*.
 Under *3D Search Paths*, add an alias *'jitter'*. **NB: in KiCAD 7 this must be in all caps 'JITTER'**. The path should be the absolute path to the *3D* folder in this repository.

 All footprints pointing to a 3d file in te format *jitter:<my3dshape.step>* should now resolve correctly.

#### Kicad 6: Fix missing 3D footprints

In Kicad 6, a lot of 3D components may not be found due to the missing variable `KISYS3DMOD`. To fix this, open the *Footprint Editor*. Go to *Preferences*, *configure paths* and add an environment variable `KISYS3DMOD`. Copy-paste the Path from `KICAD6_3DMODEL_DIR`.
