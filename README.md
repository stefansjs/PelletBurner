# PelletBurner
Pellet Burner is a 3d printer toolhead for a Voron 0 using the Greenboy3d pellet extruder hotend based on the [Dragon Burner toolhead](https://github.com/chirpy2605/voron/tree/main/V0/Dragon_Burner). The Dragon Burner

## CAD

the cad/ directory has the main fusion archive used to model the pellet burner. There is a fusion archive and two step 
files. The Pellet Burner.step file could be printed, but care needs to be taken to 

## Print Files

You need to print 4 files to use this toolhead.

  - Pellet Burner body.step OR Pellet Burner body with supports.step
  - Pellet Burner scoop, back.step
  - Pellet Burner scoop, front.step
  - Pellet Burner Tube Adapter.step

  `Pellet Burner body.step` has 2 overhangs. You can either use slicer supports, or print the `Pellet Burner body with supports.step`
  file.

  ## Alternate ducts

  The Dragon Burner has multiple ducts designed in. I imported those duct options directly into fusion. In order to 
  print the Pellet Burner with one of the Dragon Burner's alternate ducts, you'll need to open the fusion archive and 
  un-hide the ducts you want. They are all in the Pellet Burner -> DragonBurner v0.2 Ducts component. Read more about it
  in the DragonBurner repository https://github.com/chirpy2605/voron/tree/main/V0/Dragon_Burner.

  ## Current limitations

  The total height of the toolhead is quite a bit more than the default Mini StealthBurner toolhead. My configuration shows about 100mm of z travel after installing the Pellet Burner.

  The Dragon Burner has integrated support for a logo LED as well as several options for a nozzle LEDs. At the moment the Pellet Burner works but doesn't include any faceplate, so all LEDs were left out of this design. I'm not entirely sure that adding a faceplate will improve the aesthetics, but work part LED support should probably be added at some point.

  Additionally, Dragon Burner has support for several different built-in probes. At the moment the design only allows using those probes by going into the fusion model and manually exporting the pellet burner body with alternate fan ducts. This is *NOT* a drop-in replacement for the Dragon Burner since the toolhead is much taller. Any probe integrations would also need to be modified in the rest of the printer as well.

  The motor collides with corner brackets in the BoxZero build. I've included my configurations for avoiding these areas of the build plate if you also have the BoxZero corner brackets.

  ## Version History

  ### v1.0 - Initial release

  First "release" version. It is printed, tested, and working. It robs the build volume of ~20 mm of z motion. There is no documentation yet.
  