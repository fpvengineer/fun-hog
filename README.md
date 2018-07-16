# FUn HOg
<img src="/assets/hog-logo.png"/>

<hr />

## Basic Info

`FUn HOg` is a 2-2.5" freestyle frame with removable arms.  The current version is a pure x (1:1), but a lateral stretch is in the works. 

There are several configuration possible and the design is a classic "Blackout Box" format. No need for silly over engineering to generate sales.

Wait, we are not interested in selling these frames. We may, we could, but honestly we got so and tired of all the shit out there on the market (way back in 2014) we decided to design and cut our own frames.

Now the hype is worse, the noise is louder, and the intelligence behind frames lost a few more IQ points. We have no explanation as to why FPV is so fucked up, our best guess is that everyone is under the bridge huffing Scotch Guard or gasoline?!

## Configuration Range

Many different configurations are possible. 

* AUW is __100-150 gram__.
* 20 x 20 mm stack (PCB)
* 2mm hardware for PCB stack
* KV range is 4000-10000. 
* 2-4s battery @ 300-650mah
* 2-2.5" prop
* 11xx motors (going to test on 1306)
* DVR ready
* XM or similar RX
* Backpack VTX / dipole
* M3 standoffs at 20-25mm 
* 3DP camera mount needed (Nano/similar)
 
Mechanical Highlights:

* Can be built with only 2 types of cut!
* M3 hardware makes repair and upgrades easy. No need to unto down proprietary shit that will never be in stock when you need it.
* 2 or 3 plate designs allows for a heavier (3 plate) build using dual bottom plates.
* Open-source files allow the pilot to decide thickness of components.
* Plates are 100% symmetrical
* Plates are interchangeable
* Arms are removable and interchangeable

Right now, here are all __48__ different known configurations:
 
1. 2" Top mount battery
1. 2.5" Top mount battery
1. 2" Underslung battery
1. 2.5" Underslung battery
1. 2" Underslung electronics (bottom box), top mount battery
1. 2.5" Underslung electronics (bottom box), top mount battery
1. 2" Underslung electronics (bottom box), underslung battery
1. 2.5" Underslung electronics (bottom box), underslung battery
1. Narrow front (2" front, 2.5" rear arms) custom mix top mount battery 
1. Tight ass (2" rear, 2.5" front arms) custom mix top mount battery
1. Narrow front (2" front, 2.5" rear arms) custom mix underslung battery
1. Tight ass (2" rear, 2.5" front arms) custom mix underslung battery
1. __Now multiply all those configuration x 2 for dual and triple plate builds__
1. __Now multiple that AGAIN for standard plate or battery strap plate__

> __Total known configuration is 48!__  #WTF

## Suggested Configuration

There are a lot of configuration possibilities, here are 2 we like so far.

### Mellow Fellow 2"

Solid 3min flights, bigger battery suggested nonetheless.  Feels like a 5", the weight is 124.5g AUW and tames down the drivetrain a little. You have good punch, but a lower (10-15 degree) angle on the cam is recommended as this unit is designed and built to fly under cars, through windows and doors, and combine freestyle and proximity in the yard.

* 2" arms
* HGLRC stack
* RunCam backpack VTX
* RunCam Nano (actually this camera is a pile of shit and the preferred camera has no name)
* 3DP nano case
* 1104 @6500kv
* Gem Fan 2035 x 4 blade
* M3 / 25mm stack
* XM+
* ~400mah 3s (500-600 recommended)
* 2 plate build
* Top mount battery

### Bat on Fire 2.5"

Even with the lower (15 degree) angle on the camera this build gets on top of everything, your house, the trees, everything! The high RPM and bigger prop add stability and float. The longer inertial throw lends to more hang time that is stabilized by extra gyroscopic mojo form the blades.  We think this unit tops out at 50mph, but most of the time it is poking at gaps in the yard and diving the trees in range.

* 2.5" arms
* HGLRC stack
* AKK 20x20 600mw VTX 
* RunCam Nano (same disclaimer as above)
* 3DP nano case
* 1106 @ 6000kv
* Gem Fan 2.5" 2540 3-Blade Propeller 
* M3 / 25mm stack
* XM+
* ~650mah 4s
* 2 plate build
* Underslung battery

## Build Notes / Gotchas

* When purchasing an AIO ESC in a 20mm format the amp rating often differs from 30mm (spacing) boards. The difference is that the continuous and burst amp on a 20x20 are cumulative (total of all channel) and the 30x30 versions are per channel. Some known reference points for amp math:
 * 205g AUW 1306 4000k on 4s @850 using 303 Tri-props with ~200mw VTX:
     * 18-20amp to hover total, so around 4-5amp per channel
     * A punch is 35-45amp
     * Except possibly for the higher amp rated 20x20 ESC, this will fly but slowly cook and die.
 * 260g AUW 14076 @ 4000kv 3030 tri-prop 600mw vtx:
     * hovers around 25amp
     * Highest recorded burst in 82 amp, a typical punch out is 45-60amp (this drive train is serious)
 * ~110g AUV 1104 4000-7000kv range (multiple bird) 200mw vtx, 2035 or similar props:
     * Hovers around 12amp
     * Punch out gets close to 30 burst

Compare those real world numbers (not a bench test) to a typical 2200-2700kv 5" quad on medium aggressive props hovering at 20amp and punch out around 100amp. Add 25% for aggressive props, take a little off flying mellow.

Choosing the right ESC is very important. New entry to the market are not recommended, the mate may not be there when you want it. Also get a few spare ESCs provided you are in the right range.  

You are not a pussy if you put the ESC on the arm ever. Arm ESCs are generally better here is the pro/con:

* PRO:
  * Cooled naturally by prop
  * Cooler running because of separation from other gear meaning __NOT__ sandwiched between other probably hot PCBs.
  * Easier to repair generally.
  * Able to repair just one
  * Failure does not kill the whole PCB (cheaper)
* CON:
  * More wires. (not a problem if you know how to build well)
  * "prop strikes". Note the air quotes, this is not a real problem for freestyle flight.  Trying to fit through hoola hoop with 7 other buddies at the same time at full speed creates all sorts of problems. Adjust that behavior first possibly?
  * Adds mass further out from center longitudinal axis (+ inertia).  Totally true, minor hit.
  
__VTX antenna mounting__:

These little bastards don't appreciate traditional antenna mounting approaches. The best right now is a dual fatty cable tie on back stand-offs that come to a tip, like a triangle. At the end is where the di-pole should socket. Wrap with some electrical tape and done.  At lower altitude and greater distance there can be a fuzz-out zone, if you go out too far __DON'T FREAK OUT__!  If gaining altitude is a safe option, this can help sometimes, but at the risk of a bigger drop should it fail. Otherwise [tacking](https://en.wikipedia.org/wiki/Tacking_(sailing) is recommended. Simply fly about 45 degrees to the left or right of the straight line back. As needed turn the other direction 90 degrees and repeat. The zig-zag will expose the tail di-pole. 

Dipole is common for backpack VTX and generally recommended.

__Range__:

Little fuckers like the FUn HOg are generally intended for yard missions and casual Park Missile™ dog-fights.  As such __telemetry is not required__ as the ~200mw common backpack VTX takes a shit long before the data connection.   

Extending range is possible, but the size makes this difficult. More VTX kills the battery faster and generates more heat. Adding more battery and other edits turn the equation to a [red queen](https://en.wikipedia.org/wiki/Red_Queen_hypothesis) type of scenario. Frames and drive trains must achieve balance, The best balance for a 2-2.5" unit is flying in the yard or a small park. Small FPV units such as this has the power to make your surroundings much larger.  A small yard, a corner out behind where you work, or a warehouse is a great place to fly your sortie.

__Durability__:

Some of us fly these and they never break. Others are maniacs and break shit all the fucking time.  Most people are in the middle somewhere.

These units fly very fast and the impact on crash will break arms. This is a fact one much come to terms with. If a typical 5" drone travels at 40-60mph at 700g AUW and a 2" drone travels at 30+ mph ~110g AUW think about how much more force is put on the unit when making impact.

Some math via [this post](https://sciencing.com/calculate-force-impact-7617983.html).

Calculating the impact of a horizontally moving object:

```
Force in Newtons
F = (0.5 × m × v^2) ÷ d
d = .04 meter / 4cm (crumble zone)
m = weight in kilogram
v = speed in meters/second
```

__700g drone = 6.24 Newton/gram impact force__

```
F = (0.5 × m × v^2) ÷ d
4370.8 Newton = (.5 * .7 * 22.35^2) / 0.04
4371/700 = 6.24 Newton / gram
```


__110g drone = 22.36 Newton / gram impact force__

```
F = (0.5 × m × v^2) ÷ d
246.9 Newton = (.5 * .11 * 13.4^2) / 0.04
4371/700 = 22.36 Newton / gram
```

If I did my math right (correct me if wrong) the 110g drone has __3.58 times more boom on impact__. 

__DVR__:

There are a few DVR on the market at the time of this document being written.  They are NOT HD an have their own grainy vintage feel. We find it romantic and are amazed to carry onboard recording in the 100g AUW range (and larger).  Right now we have 2 different types in circulation:

* __Happy Model DVR__: Also sold by Crazy Pony and white labeled by a lot of shops.
  * 720 resolution (better)
  * 16:9 ratio compatible (thank you!)
  * AVI format
  * Only record  a few minutes (2?) and then writes and starts a new file. 
  * The small file writing will clip out about 0.5 second when the file flips looking like a glitch once edited.
  * Smaller of the units when de-cased (recommended).
  * No mounting holes. We wrap it and sticky tape it somewhere.
  * Does not auto start recording
  * Will not save if file is not finalized (written to FAT)
  * No USB, you need to pop the card
  * Runs medium hot
* __RunCam DVR__:
  * About 360 resolution. Yeah shit right?
  * Nominal 4:3 ration. Total bullshit.
  * AVI format
  * Recoding quality may be a little better, hard to say.
  * Records continuous file (so far...)
  * Auto start recording
  * 20x20 pcb, mounts on stack (like you have room?)
  * Will not save if file is not finalized (written to FAT)
  * No USB, you need to pop the card
  * Runs medium hot

## License

__CC NC-SA 4.0__

We use the Attribution-NonCommercial-ShareAlike 4.0 International (CC BY-NC-SA 4.0)license for __ONE IMPORTANT REASON__: Hobby King (and a few others). Our design is available for commercial production and we can/will cut out a license that is equitable (essentially free to you) as long as attribution is given correctly.  HK has a history of stealing design and then denying credit. As such, we would like to introduce them to a little thing called Intellectual Property rights as well as our favorite negotiation tool the baseball bat. 

Here is the basics of the license:

* __Attribution__ — You must give appropriate credit, provide a link to the license, and indicate if changes were made. You may do so in any reasonable manner, but not in any way that suggests the licensor endorses you or your use.
* __NonCommercial__ — You may not use the material for commercial purposes.
* __ShareAlike__ — If you remix, transform, or build upon the material, you must distribute your contributions under the same license as the original.

Full license here: https://creativecommons.org/licenses/by-nc-sa/4.0/.

If you want to do a production run, put some coal int eh email machine and fire it out to info@...

<img src="/assets/fh1.png"/>

<img src="/assets/fh2.png"/>
