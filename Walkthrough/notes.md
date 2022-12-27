# WOLF Tutorial Notes

## WOLF Tutorial Ships

How to keep track of which crew are required for which infrastructure lander?

Early in the game I build a lander with a detachable crew capsule. Launch the crew capsule from KSC and fly it to the lander that is built at the remote shipyard. Then dock the capsule to the lander and land it!

Later when we have WOLF passenger transport available I'll build the lander and then send the crew. It's easy enough to remember that the next crew to arrive is for the lander in orbit. It gets complicated when there are multiple passenger routes, at which point I simply have to keep the list organised by lander name:

+ 04 Twin Craters Polymers
  + Jazer Kerman
  + Maucan Kerman
  + Tevan Kerman
+ etc

Then just remember to bring the lander near the passenger terminal to transfer crew.

You can also colour code. For example some distinct colours that aren't related to navigation lights:

+ Orange (#FF7D00)
+ Teal (#19B1B2)
+ Violet (#7E00FF)

### Mun Route Builder 1

+ Canyons
+ East Farside Crater

### Mun Route Builder 3

+ Northwest Crater
+ Farside Basin

### Twiki

Northwest Crater (find a landing location)

## Preparation

Make sure that the craft can load into the stock game with only Bon Voyage and MKS/WOLF addons.

### Checklists

#### Lander Building

1. More than 100 monopropellant on station
2. Station has propellant required to fully load the lander
3. Build the lander
4. Transfer propellant
5. Move lander to parking orbit

### Route Building

1. Save game as "building route origin to destination"
2. Move all consumables (propellant, supplies, fertilizer) to nearby storage
3. Start route
4. Load consumables required for out-and-back trip (record comsumables loaded eg: delta-v for a rocket)
5. Quicksave
6. Start the outbound journey
7. Arrive at destination
8. End the route (record consumables remaining)
9. Quicksave
10. Start route
11. Start the return journey
12. Arrive at origin (record consumables remaining)
13. Load consumables required to reduce route cost to 0
14. End the route
15. Save game as "Built route A to B"

770m/s
410m/s

Greater Flats to Poles: 891 start, 492, 40

### Packaging

I'll need a Makefile to prepare a ZIP archive of:

+ Ships
+ Subassemblies
+ Save games

## Plan

+ Produce materials on Kerbin to ship to orbit
  + Material Kits
  + Fuel
  + Food
  + Fertiliser
  + Water
  + Oxygen
+ Build shipyard and send it to orbit
+ With that shipyard, build:
  + another shipyard
  + tanker
  + route builder
+ Add a resource hauler to deliver the materials for a manufacturing hopper and a depot module
+ Send that small fleet to Minmus (note staging orbit for shipyard ~800km)
+ At Minmus establish the orbital depot
+ Build the depot landers and establish all Minmus biome depots
+ Establish routes both ways between orbit and all Minmus biomes
+ Establish Material Kit manufacturing (use imported life support resources)
+ Build up local life support
+ Build up local manufacture of Specialized Parts
+ Build up local manufacture of advanced materials:
  + Alloys
  + Electronics
  + Prototypes
  + Robotics
  + Synthetics

## Shipyard Notes

### Hoppers

+ 2.5m manufacturing hopper
  + 2 WOLF Material Kit -> 2000 Material Kits/day
  + 2 WOLF Specialised Parts -> 529.1 Specialised Parts/day
  + 2 WOLF Machinery -> 529.1 Machinery/day
  + 1 WOLF Alloys -> 128.21 Alloys/day
  + 1 WOLF Electronics -> 264.55 Electronics/day
  + 1 WOLF Prototypes -> 264.55 Prototypes/day
  + 1 WOLF Robotics -> 200.00 Robotics/day
  + 1 WOLF Synthetics -> 500.00 Synthetics/day
+ 3.75m manufacturing hopper
  + 5 WOLF Material Kit -> 5000 Material Kits/day
  + 5 WOLF Specialized Parts -> 1322.75 Specialized Parts/day
  + 5 WOLF Machinery -> 1322.75 Machinery/day
  + 1 WOLF Alloys -> 384.62 Alloys/day
  + 1 WOLF Electronics -> 793.65 Electronics/day
  + 1 WOLF Prototypes -> 793.65 Prototypes/day
  + 1 WOLF Robotics -> 600 Robotics/day
  + 1 WOLF Synthetics -> 1500 Synthetics/day

### Components

Note that for the craft constructed in this walkthrough, materials are used in a highly asymmetric ratio something along the lines of:

+ 100,000 Material Kits
+ 100 Specialized Parts
+ 100 Synthetics
+ 10 Alloys
+ 1 Robotics
+ 1 Electronics
+ 1 Prototypes

In terms of hopper output, this means that to maintain production at the appropriate ratios we need the following ratio of 3.75m hoppers:

+ 12,000 Material Kit hoppers (60,000,000/day)
+ 45 Specialized Parts hoppers (60000/day)
+ 40 Synthetics hopper (60000/day)
+ 15 Alloys hoppers (6000/day)
+ 1 Robotics hopper (600/day)
+ 1 Electronics hopper (793/day)
+ 1 Prototypes hopper (793/day)

The strategy we'll apply in this walkhrough is to produce as many resources as we can from the Kerbin/Mun/Minmus system and export small quantities of everything to each other world while setting up local production. Prototypes are super-expensive to produce so they will just be shipped from KSC until there's enough production in the Kerbol system to produce them through WOLF. We barely use any Prototypes through the course of this walkthrough.

So for this walkthrough the aim with each ship yard is to have (all 3.75m components):

+ 4 Material Kits hoppers (20,000/day)
+ 1 Specialized Parts hopper (1323/day)
+ 1 Alloys hopper (385/day)
+ 1 Electronics hopper (793/day)
+ 1 Robotics hopper (600/day)
+ 1 Synthetics hopper (1500/day)

Along with those will be 4 Lf/Ox hoppers and 1 Monopropellant hopper to provide us the propellants we need for the craft we'll be building.

The broad strokes of the walkthrough strategy will thus be:

+ Establish Material Kits, Fuel, Food, Water, Oxygen production on Kerbin
+ Establish an orbital shipyard around Kerbin
+ Send a new shipyard to Minmus
+ Buy the specialized parts and advanced materials required to build Minmus Infrastructure
+ Develop Minmus Infrastructure to produce 10 WOLF Material Kits, 5 WOLF Specialized parts, and 1 each of the advanced materials to support local production
+ Further develop Minmus to export some useful resources
+ Repeat the expansion with Mun starting with a ship yard, then deploying depots to bring advanced materials production up to speed for self-sufficiency
+ Repeat that expansion with Duna

Total production required from Minmus will then be the minimum required to run 1 3.75m hopper of each building material (but not Prototypes):

1. Material Kits x 25 (15 + 5 + 5)
   + Chemicals x 25 (1 x 25)
   + Metals x 50 (2 x 25)
   + Polymers x 50 (2 x 25)
2. Specialized Parts x 5
   + Refined Exotics x 10 (2 x 5)
     + Exotic Minerals x 20 (2 x 2 x 5)
     + Rare Metals x 30 (3 x 2 x 5)
   + Silicon x 15 (3 x 5)
3. Alloys x 6 (1 + 5)
   + Metals x 6 (1 x 6)
   + Rare Metals x 24 (4 x 6)
4. Synthetics x 6 (1 + 5)
   + Exotic Minerals x 24 (4 x 6)
   + Polymers x 6 (1 x 6)
5. Electronics x 1
   + Material Kits x 5
   + Synthetics x 5
6. Robotics x 1
   + Alloys x 5
   + Material Kits x 5

The sum total thus becomes:

+ Chemicals x 25 (only for MK)
+ Exotic Minerals x 44 (20 for SP + 24 for Synthetics)
+ Metals x 56 (50 for MK + 6 for Alloys)
+ Polymers x 56 (50 for MK + 6 for Synthetics)
+ Rare Metals x 54 (30 SP + 24 for Alloys)
+ Silicon x 15 (only for SP)

This will be enough to support production up until around the point we have a thousand Material Kits hoppers.

Note that _Material Kits_ and _Specialized Parts_ are also required for _Colony Supplies_ and _Machinery_. _Colony Supplies_ are required to manage passenger routes in WOLF, and apart from being required for _Colony Supplies_, _Machinery_ is only used in MKS.

#### Expansion Shipyard

+ 123,533 Material Kits
+ 948 Specialized Parts
+ 265 Alloys
+ 533 Synthetics
+ 63 Robotics

Note that the Duna Shipyard comes with hoppers for Material Kits, Specialized Parts, LF/O and Monopropellant. With a small amount of extra supplies this shipyard can build the A/E/S/R hopper and then start "producing" A/E/S/R locally.

#### A/E/R/S Hopper

+ 32230 Material Kits
+ 369 Specialised Parts
+ 94 Alloys
+ 145 Synthetics
+ 20 Robotics

#### Fuel Hopper

+ 34,782 Material Kits
+ 186 Specialized Parts
+ 53 Alloys
+ 144 Synthetics
+ 20 Robotics

#### Minmus Depot Lander

+ 18,135 Material Kits
+ 74 Specialized Parts
+ 27 Synthetics
+ 1 Robotics

#### Route Builder Rover

+ 65,408 Material Kits
+ 542 Specialized Parts
+ 155 Alloys
+ 37 Synthetics
+ 3 Robotics

### Minmus Budget

To build the Minmus shipyard we'll need:

+ Expansion Shipyard (comes with MK, Sp, propellant hoppers)
+ Satellite Bundle (88Sp, 51A, 13S, 2R)
+ A/E/R/S Hopper (31,722MK, 353Sp, 94A, 145S, 20R)
+ Skycrane Depot Box x 8 (5570MK, 68Sp, 18A, 51S, 1R)
+ Skycrane (11,195MK, 86Sp, 30A, 5S, 1R)
+ 01 Greater Flats Alloys
+ 02 Lowlands Synthetics
+ 03 Greater Flats Material Kits
+ (5 specialized parts?)
+ (1 robotics?)
+ (1 electronics?)

+ 948 + 353 + (74*8) + 542 = 2435 Sp
+ 265 + 94 + 0 + 155 = 514 A
+ 63 + 20 + 8 + 3 = 94 R
+ 533 + 145 + (27 * 8) + 37 = 931 S

Minmus is a pain to navigate by rover. My Route Builder Rover slides over most terrain and the USI rover wheels are broken. Thus expansion on Minmus will be by rocket.

On Minmus we'll need to find depots that can most easily fill the production requirements for:

+ Specialized Parts
+ Synthetics
+ Alloys
+ Robotics
+ Electronics
+ and Material Kits last due to having supply from Kerbin

Depot candidates:

+ Flats
  + 5 Material Kits
+ Great Flats
  + 5 Alloys
  + 70 Rare Metals
  + 45 Silicates
  + import substrate for Material Kits
+ Greater Flats
  + 50 Material Kits
  + 5 Alloys
  + 30 substrate
+ Highlands
  + 15 material Kits
  + 1 Alloys
+ Lesser Flats
  + 1 Alloys
+ Lowlands
  + 30 Exotic Minerals
  + 20 Food
  + 60 Water from Hydrates
  + 7 Synthetics locally if it consumes its own polymer and exotic minerals production
+ Midlands
  + 90 Exotic Minerals
  + Food
  + Fertilizer
  + Water
+ Poles
  + 40 Exotic Minerals
  + 40 Fertilizer
  + import 8 substrate to make Material Kits

With 24 Exotic Minerals to import, Greater Flats can then produce 20 Specialized Parts and 2 Synthetics.

So rough plan:

+ Greater Flats for Alloys, some Material Kits
+ Lowlands for Food, Water, 1 Synthetics for Minmus Station, Exotic Minerals
+ Midlands for Exotic Minerals, Food, Water, Fertilizer
+ Poles for Exotic Minerals
+ Greater Flats for Synthetics
+ Great Flats for Alloys
+ Further depot expansion to extract remaining exotics, rares, polymers, metals

## Mun

### Depot Candidates:

+ Alloys
  + East Farside Crater (Alloys, Robotics, Food, Fertilizer, Water)
+ Electronics
+ Robotics
+ Synthetics



## Passengers to Orbit

 54 passengers (6 * 9) requires:

+ 108 extra habitation
+ 108 extra life support
+ 4 food, 4 oxygen, 20 water

Note that some addons will prevent routes showing up. My list of suspects that I haven't delved into further:

+ MechJeb 2
+ Docking Port Alignment Indicator
+ Kerbal Alarm Clock

## Screenshots required

## Locations

### Kerbin

+ KSC/right next to Kerbal centre (-0.1, -74.647)
+ KSC/Shores Just north of runway (-0.04, -74.709)
+ Grasslands (0.0 -75.38)
+ Highlands (1.741, -77.339)
+ Mountains (0.637, -78.659)
+ Desert (1.472, -86.435)
+ Ice Caps (71.386, -92.709) which needs a waypoint around (36.898, -63.906) on the way there and back to constrain the route finding

### Minmus

+ Midlands (4.390, -86.594) or (4N, 86 43'37"W) -- flat plateau to the immediate east of Great Flats
+ Greater Flats (0, -7.5) or (0N, 7 30'00"W)
+ Flats (1.5, -40) or (1 30' 0"N 40 0' 0"W) -- bottom lobe of the flats just NW of Greater Flats
+ Lesser Flats (9.404, -178.003) (9° 24' 14.4"N, 178° 0' 10.8"W)
+ Great Flats (-10, -92) (10S, 92W)
+ Poles (78.045, 164.276) (78° 2' 42"N, 164° 16' 33.6"E)
+ Lowlands (0.026, -51.516) (0° 1' 33.6"N, 51° 30' 57.6"W)
+ Highlands (0N, 82E)

Satellites:

+ Synchronous orbit: 357940.87 (40400s)
+ Deployer apoapsis: 534657.74 ()
+ "Low" orbit is 10-20km

+ Shipyard Component
  + 42,400 _Material Kits_
  + 528 _Specialized Parts_
  + 145 _Alloys_
  + 194 _Synthetics_
+ A/E/R/S
  + 32,230 _Material Kits_
  + 369 _Specialized Parts_

### Mun

+ Canyons (18.150, -50,300) (18 9' 0"N, 50 18'0"W) (18.177, -50.448)
+ East Crater (-0.617, 81.593)
+ East Farside Crater (7.109, -150.838)
+ Farside Basin (29.618, -93.351) (29 37' 5"N, 93 21' 5"W)
+ Farside Crater (-0.247, -58.873) (0 14' 48"N, 58 53' 2"W)
+ Highland Craters (64.424, 173.655) (64 25' 41"N 173 40' 3"E)
+ Highlands (0.372, -34.280)
+ Lowlands (0.305, -0.530) (0 18'18"N, 0 31'48"W)
+ Midland Craters (4.542, 43.048) (4 32'31"N, 43 2'59"E)
+ Midlands (0,96.966) (0N, 96 58'20"E)
+ Northern Basin (36.592, 61.975) (36 35'34"N, 61 58'47"E)
+ Northwest Crater
+ Polar Crater (50.87, -36.55) (50 52' 4"N 36 32' 59"W)
+ Polar Lowlands (79.666, 108.266) (79° 39' 57.6"N, 108° 15' 57.6"E)
+ Poles (74.464, 83.926) (74 27'56"N, 83 59'3"E)
+ Southwest Crater
+ Twin Craters (-5.916, 139.817) (5 54'56"S, 139 49' 1"E)

Satellites:

+ Synchronous orbit is not possible
+ Satellite orbit:
+ Deployer apoapsis:
+ "Low" orbit is under 60km

### Duna

+ Lowlands (10.199, 78.161)
+ Northern Shelf (43.572, 37.790)

### Eve

+ Shallows (-55.060, 113.400 - near Western Sea)

Survey altitude is 1000km (70km to 1500km).

## Uraninite For Nuclear Reactor Fuel

+ Mun, Farside Crater 6.76% (2.943, 61.761)

## Bon Voyage

+ RotationVector
  0. "up" sitting on nose
  1. "down" sitting on rear clamp-o-tron Sr
  2. "forward" right way up

## To Do

+ Extract list of screenshot names from wiki_page.md
+ Figure out a Markdown notation to provide the caption and filename for each screenshot
+ Find or build a tool to build TOC from Markdown headings
+ Find or build a tool to generate table of illustrations
+ Resource conversion table listing the producer that you can get desired materials from (ie: one column for a resource, second column showing which modules have the recipe)
+ Pictures of each location
  + from orbit to give an overview
  + from destination to show specifics
+ Include the route building in the walkthrough specifically
+ Upgrade to Orbital Route Builder 75 earlier in Minmus campaign
+ Merge the walkthrough with the save game repository

## References

[KSPFORUMMKS]: https://forum.kerbalspaceprogram.com/index.php?/topic/154587-111x-modular-kolonization-system-mks/ "KSP Forum: MKS Announcement Thread"
[WOLFIWPC]: https://github.com/UmbraSpaceIndustries/MKS/wiki/WOLF-%E2%80%94-Industry-without-the-part-count "WOLF: Industry without the part count"
[MRWOLFTS]: https://github.com/MaraRinn/WOLF-Tutorial-Ships "Mara Rinn's WOLF Tutorial Ships repository"
[BCRESDIAG]: https://forum.kerbalspaceprogram.com/index.php?/topic/154587-111x-modular-kolonization-system-mks/&do=findComment&comment=4026544 "bigcalm's resource diagram"
[DECDEGREES]: https://www.rapidtables.com/convert/number/degrees-to-degrees-minutes-seconds.html "Decimal Degrees to Degrees,Minutes,Seconds"
[ALARMENHANCE]: https://github.com/severedsolo/AlarmEnhancements/releases "KAC-style enhancements for stock alarm clock"