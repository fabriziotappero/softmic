
# Software Microphone

This repository is the home of *Software Microphone*, a high-quality wireless 
microphone. Here everything is open sourced: schematics, circuit simulations, 
mechanical drawings and software code.

## Folder Structure
This is the folder structure of this project.
```
root
│   README.md               The file your are reading
│   license.md              License file    
└───sch                     Schematics and PCB fab files done in KiCad
│   │   softmic.pro
│   │   softmic.sch
│   │   softmic.kicad_pcb
│   └───lib                 Kicad library files
│   └───pdf                 IC data sheets
└───sim                     Simulated circuits in LT Spice
│   │   softmic-sim.asc
│   └───lib                 LT Spice library  
└───src                     Micropython ESP32 code
└───mec                     Mechanical parts designed in Blender
└───img                     Various images
└───tmp                     generic data sheets and additional info
```
## Starting point
I actually own a [Samson C02](https://www.amazon.com/s?k=samsons+c02) condenser
microphone that I use together with a [Tascam DR-40](https://www.amazon.com/s?k=tascam+dr-40).
[Here](https://soundcloud.com/cinema_sound/samson-c02-dx-pop-filter) an example of what the Samson C02 sounds like 
and here is the picture of the inside of the Samson C02.

<p align="center">
  <img src="https://github.com/fabriziotappero/softmic/blob/master/img/samson-c02.jpg?raw=true" alt="" width="90%"/>
</p>
Here you can see the actual schematic of the Samson C02. Nothing really mind-blowing but functional.
<p align="center">
  <img src="https://github.com/fabriziotappero/softmic/blob/master/img/samson-c02-schematic.jpg?raw=true" alt="" width="90%"/>
</p>

For the time being this is the starting point of this project. The objective of this project is to make something of a 
similar quality but wireless.

## Schematics
In the following figure you can see the KiCad schematic of softmic done in KiCad.

<p align="center">
  <img src="https://github.com/fabriziotappero/softmic/blob/master/img/softmic-schematic.jpg?raw=true" alt="" width="90%"/>
</p>

## Mechanical Parts
A full fledged microphone is not only made of its electronics, mechanical parts 
are equally important.

Any mechanical parts in this projects are made with non-destructive modeling 
using [Blender](https://www.blender.org) version 2.8. 
For a quick start have a look at this [great tutorial](https://www.youtube.com/watch?v=WzwmkYhlrcQ).

## License
Copyright (c) 2020 Fabrizio Tappero

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

## References
A lot of microphone and microphone-related products and devices exists out there.
Here is what it can be considered a good starting point.

[Electret microphone](ttps://sound-au.com/articles/mic-electret.htm) and their
[electret Capsule](http://www.firstpr.com.au/rwi/mics/2009-09-a/).

[Microphone capsule Manufacturer](https://www.jlielectronics.com/microphone-capsules/?sort=pricedesc)
and one more [ capsule Manufacturer](https://microphone-parts.com/collections/capsules).

[Extensive RODE guy lecturer](https://www.youtube.com/watch?v=yKOH0DyRWRU&list=PLHoGZ7nuFTo8VmQBhzZxl-qDEIN7T5Vt8).
and some [audio Microphone Kits](https://microphone-parts.com/collections/mod-kits).

[Electret Amplifier Circuits](http://xtremecircuits.blogspot.com/2012/09/compressor-for-electret-microphone.html).

Some Texas instruments IC, [here](https://www.ti.com/lit/an/sboa320a/sboa320a.pdf) and 
[here](http://www.ti.com/lit/ug/tidu765/tidu765.pdf).

if you google *TS971 based Electret Condenser Microphone Amplifier* you get:
[this](https://robbietrumpet.com/soundcatchers.net/studio_recording_sound.htm), 
[this](https://www.instructables.com/id/Modify-a-cheap-LDC-Condenser-microphone/), 
[this](http://www.sdiy.org/oid/mics/Schoeps.gif) and 
[this](http://www.zen22142.zen.co.uk/Circuits/Audio/ecmmic.htm).

[Some electret capsules](https://www.abcomponents.co.uk/product-category/electret-microphones/) and 
[this](https://micbooster.com/12-primo-microphone-capsules) and 
[this](https://micbooster.com/content/12-comparison-table-for-primo-microphone-capsules).

Very interesting [electret capsules](https://micbooster.com/primo-microphone-capsules/9-em173.html)
and [some more](https://micbooster.com/primo-microphone-capsules/8-primo-em172.html) plus the 
[very best electret capsule](http://www.micbooster.com/documents/EM173%20Oct%202011.pdf).

[Application Note about LSK489](http://www.linearsystems.com/lsdata/others/LSK489_Application_Note.pdf).

[Interesting capacity multiplier](http://www.audioimprov.com/AudioImprov/Mics/Entries/2014/12/18_Another_Chinese_mic_Circuit.html).


[Samson C02 internal circuit](http://www.audioimprov.com/AudioImprov/Mics/Entries/2015/4/23_Basic_FET_Microphone_Circuits.html).

[Popular Alice schematic](http://scotthelmke.com/alice-mic.html).

[How to bias a JFET](http://www.vishay.com/docs/70595/70595.pdf).

[Audio compressor](https://www.electroschematics.com/audio-compressor-agc/).

[Audio Op Amp IC from Texas Instrument](http://www.ti.com/lit/ds/symlink/opa1678.pdf).

Interesting [blog post](https://www.diyaudio.com/forums/equipment-and-tools/319784-search-ultra-quality-electret-mic-interface-circuit.html) and 
[here](https://www.electronics-lab.com/project/low-noise-mini-electret-microphone-preamplifier/),
[here](http://www.johncon.com/john/wm61a/) 
and [here](http://www.micbooster.com/documents/EM173%20Oct%202011.pdf).

[Interesting audio people](https://micbooster.com/)

[Interesting microphone case](https://eu.mouser.com/Wire-Cable/Wire-Cable-Management/Cable-Glands-Strain-Reliefs-Cord-Grips/_/N-fb8zo) and [one more](https://eu.mouser.com/datasheet/2/18/inhouse_Amphenol_C146%20Series_Accessories_VN16-1158081.pdf).

[Audio Preamp product](https://www.bhphotovideo.com/c/product/292989-REG/Sound_Devices_MM_1_MM_1_Single_Channel_Portable.html/overview) and one more 
[reference audio preamp](http://www.hiroshi.com.hk/en/product/detail/mini-microphone-pre-amplifier-23#.Xn4073Io_ws)
that I actually own.