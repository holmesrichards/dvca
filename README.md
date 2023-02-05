This is a work in progress; better README to come soon. Meanwhile:

**Untested hardware and software — Do not assume anything works!**

# MFOS Dual VCA

Kosmo format version of the Music From Outer Space Dual VCA synth module.

## Current draw
?? mA +12 V, ?? mA -12 V


## Photos

![]()

![]()

## Documentation

* [Schematic](Docs/dualvca.pdf)
* PCB layout: [front](Docs/dualvca_layout_front.pdf), [back](Docs/dualvca_layout_back.pdf)
* [BOM](Docs/dualvca_bom.md)
<!-- * [Build notes](Docs/build.md) -->
<!-- * [How it works](Docs/howitworks.md) -->
<!--* [Blog post]() -->

## GitHub repository

* [https://github.com/holmesrichards/dvca](https://github.com/holmesrichards/dvca)

## Submodules

This repo uses submodules aoKicad and Kosmo_panel, which provide needed libaries for KiCad. To clone:

```
git clone git@github.com:holmesrichards/dvca.git
git submodule init
git submodule update
```


Alternatively do

```
git clone --recurse-submodules git@github.com:holmesrichards/dvca.git
```

Or if you download the repository as a zip file, you must also click on the "aoKicad" and "Kosmo\_panel" links on the GitHub page (they'll be in the Libraries folder and will have "@ something" after them) and download them as separate zip files which you can unzip into this repo's aoKicad and Kosmo\_panel directories (in the Libraries folder).

If desired, copy the files from aoKicad and Kosmo\_panel to wherever you prefer. 

Then in KiCad, go into Edit Symbols and add symbol libraries 

```
aoKicad/AO_symbols
Kosmo_panel/Kosmo
```
and go into Edit Footprints and add footprint libraries 
```
aoKicad/AO_tht
Kosmo_panel/Kosmo_panel.
```

