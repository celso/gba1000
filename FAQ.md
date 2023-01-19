# FAQ

Information copied from the old gba1000.info website, and more.

## Difficulty of building a GBA1000

***"I do not want to deal with frustrated people who participate in a bulk order because of a good price, especially when it results in nasty comments on the web. Completing the board requires about 20 to 30 hours of soldering including work on rosters with pin distances of 0.5 mm. The circuit is highly complex and involves many potential sources of error. Troubleshooting involves working with oscillators, drivers and custom chips bought as "new", which for one reason or another may not work properly. Soldering problems also occur, which happen to me too. Debugging can easily take several hours. On top of that, you will be working with a 4 layer PCB, which of course must be of suitable quality, including the size of the PCB, through-layer contacts and minimum measure. Also, a good free of debris adhesion of the copper layer is needed for the visa and IC-sockets etc. The solder mask must be resistant to solder running on to it and the PCB should not show any bends or twists. Some of the components used in this board are difficult to obtain or only obtainable from older Amiga hardware. This does not only concern the Amiga custom chips but also TTL-Gutter like for instance 74F245 which is no longer in trade in an SMD model. The project builder must know where to find these parts on his own."***

## Order to populate the board:

***Schneemann: I am not afraid to solder the board, but I'm worrying getting stuck in case of any error. It will be not my first PCB, but the first of that size and complexity. I hope that it will be possible to set up the board step by step, as far as Georg just "easily" integrated the IDE-controller and the flicker fixer via (not directly visible) standard Amiga-interfaces. That means the main-part should work even without flicker fixer and IDE-controller. If I'm right, most of the GALs belong to these optional parts. The CPU, FPU and custom chips are socketed (easy to check). More difficult is the RAM (hard to solder and getting damaged fast), but if this part works, we should see a picture, e.g. with an external flicker fixer, on the screen, then the rest could follow.***

***Kristian95: You are right there are many possibilities for errors and trouble shooting will most likely take most of use as much time as the actual soldering. The Flicker fixer is indeed optional (no changes necessary to the build if you leave it out). Also the IDE controller is optional, I can't remember what change you need to make to the build, but it is documented in my translation of the user's guide. I don't think it should be a big problem getting the GALs programmed. Do you know whether it would be "easy" to make the RAM socketed instead of surface mounted? If it is we might consider doing so :) Therefore we should find such kind of build-phases in order to have chance of any testing.***

***Schneemann: The GALs are not the problem. It is in general better to have parts of the board tested and running well before starting with other parts and unfortunately, you can't test the IDE controller and the flicker fixer (that's where the GALs are used) without the CPU and RAM working. So I suggest the best build order is vice versa, i.e. leave most of the GALs as well as SD and IDE for later and start by building and testing the bare computer.***

## Soldering work

**During the soldering work, I'm afraid of getting stuck in case of errors. Any ideas?**

Gleaming from the discussion above:
* The soldering process can be divided into steps.
* Consider integrating the flicker fixer and the IDE controller after the main part works.
* Main part CPU, FPU and custom chips are socketed.
* GAL chips, perhaps most challenging, are seemingly on optional video and IDE parts.
* Solder RAM later, after the board produces a picture on an external flicker fixer.

In short, build the main board first. Add the RAM, flicker fixer and IDE controller when you've tested that the main board works.

**I'm afraid to dammage parts during the soldering. Any suggestions?**

* True, this is not going to be easy.
* Practice on old parts first. (I purchased cheap electronics at second hand shops for this purpose.)
* Watch the soldering videos listed in the links section.
* Purchase a good soldering station. See the one suggested by Plaz listed in the links section.
* More information about tools will be listed as it becomes available from experienced members.

**Another soldering tip...**

When assembling the board solder the FlashROM as the very last thing. The reason is that the space between the pins is very short there and it is therefore the easy place to make a solder bridge. Thus if you test the board prior to soldering the FlashROM and the board works, and then it doesn't work after the FlashROM is soldered, you made your error finding much easier.

## Board's parameters

```
4 Layer (35µm , 35µm , 35µm , 35µm)
1x Materials (FR4 0,71 35/35)
4x Prepreg (7628,7628,7628,7628)
Thickness: 1.54mm
Panel size: 344.488mm x 314.007mm

4648 Drills. / Panel.
21 Drill changes
Smallest drill Ø: 0.3mm
Technology: >= 150µm
SMD: doppelseitig >= 1/50"
Finish: chem. Ni/Au
Soldermask: on both sides
Identprints: 1
Peel off mask: no
Mech. working: Fräsen;
E-Test: Yes
```

