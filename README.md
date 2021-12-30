# PrintrbotSME3DV6_wHtdBed
Repo for my Printrbot Simple Metal that's heavily modded.

The Printrbot Simple Metal is a great printer, there are just a few things to bring it current. Some of my mods to do just that:
- [E3D V6 hot end](https://www.matterhackers.com/store/l/v6-hotend-full-kit-1.75mm-universal/sk/M4UK0AVU). See my [blog](https://designbuildfix.blogspot.com/2019/05/printrbot-simple-metal-e3d-upgrade.html) regarding installation and notes.
- Octoprint server running on a Pi Zero. [Blog post](https://designbuildfix.blogspot.com/2019/11/pi-zero-w-octopi-printrbot-simple-metal.html)
- ATX PSU with remote on/off through OctoPrint. [Blog post](https://designbuildfix.blogspot.com/2020/06/atx-psu-for-3d-printer.html)
- Heated bed with boro glass+PEI surface. Blog post in the works!
- Z-Axis endstop which replaced the inductive probe. The glass bed prompted the shift away from the inductive probe and a capacitive probe I was trying out wasn't accurate enough to level the bed correctly. Blog post in the works!
- [Bed FET](https://digital-sqrt.com/product/little-driver-1-9b-900watt-heated-bed-hot-end-power-mosfet-expansion-module/). This takes the load off of the Printrboard. JST pins are not meant to handle that kind of current. Don't buy the bottom of the barrel FETs off of Alibaba or Amazon. They're large, low quality, and less efficient. 

<p align="center">
  <img width="600" height="400" src="https://i.imgur.com/2tFE3qf.jpg">
</p>

There are quite a bit of firmware changes that are required for some of these modifications to work. I'll be archiving my changes here as I continue building for someone else that would like to upgrade their Printrbot!

I'm compiling my code using Arduino 1.8.11 for simplicity. You'll need to install the Teensyduino add on for the Arduino IDE if you wish to do this. I outline some of these instructions in my blog post on the E3DV6 upgrade. Definitely tune your extruder and bed PIDs on your own, never trust anyone elses!
