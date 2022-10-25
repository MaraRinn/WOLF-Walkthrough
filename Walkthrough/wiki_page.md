# WOLF Walkthrough -- Industry Without the Part Count <!-- omit in toc -->

- [WOLF From Scratch: Introducing WOLF Infrastructure on Kerbin](#wolf-from-scratch-introducing-wolf-infrastructure-on-kerbin)
- [Goals](#goals)
- [Housekeeping](#housekeeping)
  - [WOLF for the Adventurous](#wolf-for-the-adventurous)
  - [WOLF Resource Conversions](#wolf-resource-conversions)
  - [The Plan](#the-plan)
- [Prepare The Walkthrough Game](#prepare-the-walkthrough-game)
  - [Install the requried Addons](#install-the-requried-addons)
  - [Pre-Packaged Save Game](#pre-packaged-save-game)
- [WOLF Biomes](#wolf-biomes)
  - [WOLF Route Builder Rover](#wolf-route-builder-rover)
  - [Surveying Harvestable Biome Resources](#surveying-harvestable-biome-resources)
- [WOLF Dashboard -- Harvestable Resources and Depots](#wolf-dashboard----harvestable-resources-and-depots)
- [WOLF Modules](#wolf-modules)
  - [Establish KSC Depot](#establish-ksc-depot)
  - [WOLF Infrastructure Expansion](#wolf-infrastructure-expansion)
  - [Adding Production to WOLF Depots](#adding-production-to-wolf-depots)
  - [01 Grasslands Material Kits](#01-grasslands-material-kits)
  - [02 Shores Fuel and Life Support](#02-shores-fuel-and-life-support)
- [WOLF Routes](#wolf-routes)
  - [WOLF Transfers](#wolf-transfers)
  - [Transport Routes and Transport Credits Costs](#transport-routes-and-transport-credits-costs)
  - [Quick and Dirty Transport Credit Example Flights](#quick-and-dirty-transport-credit-example-flights)
  - [Transport Module for Transport Credits](#transport-module-for-transport-credits)
  - [How To Avoid Transport Credit Costs of Propellant-Consuming Vehicles](#how-to-avoid-transport-credit-costs-of-propellant-consuming-vehicles)
- [Bootstrapping Kerbin Orbit WOLF Infrastructure](#bootstrapping-kerbin-orbit-wolf-infrastructure)
  - [Commission Kerbin Shipyard](#commission-kerbin-shipyard)
- [Extracting Resources from WOLF to MKS](#extracting-resources-from-wolf-to-mks)
  - [Establishing the Kerbin Shipyard](#establishing-the-kerbin-shipyard)
  - [Crew Transport Preparation](#crew-transport-preparation)
- [Minmus Expansion](#minmus-expansion)
  - [Minmus Shipyard](#minmus-shipyard)
  - [Minmus Overview](#minmus-overview)
  - [Minmus CommNet and Skycrane](#minmus-commnet-and-skycrane)
  - [Minmus Route Preparation](#minmus-route-preparation)
  - [01 Midlands Exotic Minerals](#01-midlands-exotic-minerals)
  - [02 Greater Flats Synthetics](#02-greater-flats-synthetics)
  - [03 Midlands Agricultural Support](#03-midlands-agricultural-support)
  - [04 Greater Flats Food and Electronics](#04-greater-flats-food-and-electronics)
  - [05 Greater Flats Robotics](#05-greater-flats-robotics)
  - [06 Lowlands Polymers](#06-lowlands-polymers)
  - [07 Flats Stage 1](#07-flats-stage-1)
  - [08 Highlands Material Kits](#08-highlands-material-kits)
  - [09 Greater Flats Material Kits](#09-greater-flats-material-kits)
  - [10 Poles Exotic Minerals](#10-poles-exotic-minerals)
  - [11 Midlands Exotics and Food](#11-midlands-exotics-and-food)
  - [12 Great Flats Specialized Parts](#12-great-flats-specialized-parts)
  - [13 Flats Chemicals and Silicon](#13-flats-chemicals-and-silicon)
  - [14 Great Flats Rare Metals](#14-great-flats-rare-metals)
  - [15 Highlands Rare Metals](#15-highlands-rare-metals)
  - [16 Greater Flats Industry Park (teal)](#16-greater-flats-industry-park-teal)
  - [17 Great Flats Fuel (violet)](#17-great-flats-fuel-violet)
  - [18 Flats Fuel (orange)](#18-flats-fuel-orange)
  - [19 Highlands Life Support](#19-highlands-life-support)
  - [20 Midlands Metals (teal)](#20-midlands-metals-teal)
  - [21 Lesser Flats Silicon (violet)](#21-lesser-flats-silicon-violet)
  - [22 Greater Flats Specialized Parts (orange)](#22-greater-flats-specialized-parts-orange)
  - [Build Routes Back to Kerbin Orbit](#build-routes-back-to-kerbin-orbit)
- [Passenger Transport](#passenger-transport)
  - [Passengers from KSC to Kerbin Orbit](#passengers-from-ksc-to-kerbin-orbit)
  - [03 Grasslands Material Kits](#03-grasslands-material-kits)
  - [04 Grasslands Material Kits](#04-grasslands-material-kits)
  - [05 KSC Colony Supplies](#05-ksc-colony-supplies)
  - [Establish KSC to Orbit Passenger Route](#establish-ksc-to-orbit-passenger-route)
  - [Passenger Transfers](#passenger-transfers)
  - [06 Grasslands Material Kits](#06-grasslands-material-kits)
  - [07 Orbit Colony Supplies (SPH)](#07-orbit-colony-supplies-sph)
- [The Mun Expansion](#the-mun-expansion)
  - [Mun Shipyard](#mun-shipyard)
  - [Mun CommNet](#mun-commnet)
  - [Mun Passenger Routes](#mun-passenger-routes)
  - [Mun Depots](#mun-depots)
  - [Mun Route Builder Rover](#mun-route-builder-rover)
  - [Depot Deployment Checklist](#depot-deployment-checklist)
  - [01 Farside Crater Material Kits](#01-farside-crater-material-kits)
  - [02 Highlands Specialized Parts](#02-highlands-specialized-parts)
  - [03 East Farside Polymers](#03-east-farside-polymers)
  - [04 Twin Craters Polymers](#04-twin-craters-polymers)
  - [05 Canyons Exotic Minerals](#05-canyons-exotic-minerals)
  - [06 Farside Basin Material Kits](#06-farside-basin-material-kits)
  - [07 Canyons Electronics and Robotics](#07-canyons-electronics-and-robotics)
  - [08 Twin Craters Material Kits](#08-twin-craters-material-kits)
  - [09 East Farside Crater Rare Metals](#09-east-farside-crater-rare-metals)
  - [10 Farside Crater Specialized Parts](#10-farside-crater-specialized-parts)
  - [11 Highlands Specialized Parts](#11-highlands-specialized-parts)
  - [12 Polar Crater Exotic Minerals](#12-polar-crater-exotic-minerals)
  - [13 Farside Crater Colony Supplies](#13-farside-crater-colony-supplies)
  - [14 East Crater Exotic Minerals](#14-east-crater-exotic-minerals)
  - [15 Farside Crater Water](#15-farside-crater-water)
  - [16 East Farside Polymers](#16-east-farside-polymers)
  - [17 Farside Crater Prototypes](#17-farside-crater-prototypes)
  - [Wrapping Up](#wrapping-up)
- [Duna Expansion](#duna-expansion)
  - [Relay Satellites](#relay-satellites)
  - [Establish Depots](#establish-depots)
  - [01 Midland Sea Material Kits](#01-midland-sea-material-kits)
  - [02 Polar Craters Metals](#02-polar-craters-metals)
  - [03 Midland Sea A/E/R/S](#03-midland-sea-aers)
- [WOLF Walkthrough Conclusion](#wolf-walkthrough-conclusion)
- [Addendums](#addendums)
  - [Route Builder Rover User Guide](#route-builder-rover-user-guide)

## WOLF From Scratch: Introducing WOLF Infrastructure on Kerbin

WOLF is an industry-focused extension to the industrial activities enabled in the Modular Kolonisation System. In typical mid- to late-game save files using MKS, you will have hundreds of MKS modules scattered about the place, with your planetary maps littered with various mining, refining or manufacturing facilities.  All of these facilities and the per-tick or per-second calculations they require place significant load on the KSP simulation, and loading up the models when they get in physics range can produce significant lag in the graphics engine.

The idea with WOLF is to provide the same industrial capability as MKS without the part count, without the lag, and without endless futzing around with manufacturing lines to get everything working the way you expect it to (including, for example, having to visit each industry site every few days to "catch up" with production that was supposed to happen in the meantime).

WOLF is intended as an enhancement to MKS industry — even if you haven't got enough parts in your infrastructure to invoke the Kraken, WOLF can still be handy for you by providing part-free and attention-free resource production and transfers between biomes on the same world, between surface and orbit, and between worlds.

## Goals

The in-game goals for the walkthrough are roughly:

1. Introduce you to WOLF infrastructure on Kerbin
2. Bootstrap WOLF infrastructure on Minmus using resources exported from Kerbin
3. Bootstrap WOLF infrastructure on Mun using resources from Minmus
4. Bootstrap WOLF infrastructure on Duna using resources and advanced materials exported from Kerbin/Minmus/Mun

These stages will go from the basic WOLF industry supported on Kerbin to more advanced industry on Minmus, then expansions to Mun and Duna showing how to start a new mid- to late-game industrial expansion using WOLF.

## Housekeeping

### WOLF for the Adventurous

RoverDude wrote up [this introduction to WOLF][RDWOLF1] which outlines most of what you need to know to get started. There's also RoverDude's [explanation of transport routes and transport credits][RDTRAN1] which will be expanded upon in this walkthrough. This walkthrough really only restates what is written there with a few step by step examples and an end goal of manufacturing spaceships at an orbital shipyard and expanding infrastructure to Minmus, Mun, and Duna.

### WOLF Resource Conversions

There are a number of differences in the resource chain between MKS and WOLF, check [RoverDude's resource conversion diagram][RDCONV] for the details.

### The Plan

For this part of the walkthrough, the focus is on introducing the WOLF components and workflows through a "go big up front" campaign:

1. Explore WOLF biomes and depots
2. Introduce WOLF transport routes and shipments
3. Prepare the infrastructure to support expansion to Minmus
4. Expand to Minmus using WOLF cargo routes with crew being transported in stock/MKS craft
5. Expand to Mun using WOLF passenger and cargo routes
6. Expand to Duna using WOLF passenger and cargo routes

The Duna expansion will take all the lessons learned from the Mun expansion and simply reapply them. One aim of this walkthrough is to use a relatively small fleet of vessels to complete the walkthrough.

Throughout this guide you'll see reference to PAW, which is the "Part Action Window" that you typically open up by right-clicking on a part.

## Prepare The Walkthrough Game

There's a bit of housekeeping to take care of before you can start the walkthrough proper:

1. Some add-ons to install
2. A pre-packaged savegame to copy

### Install the requried Addons

Before you start a new KSP game, you'll need to install the Umbra Space Industries add-ons that make MKS and WOLF work:

1. Download the [Umbra Space Industries add-on collection][USIRELEASES] - this walkthrough is based on the "Stable Release 2022.5.29" package released 30 May 2022
2. Open that USI archive and copy all the things inside the GameData folder into the KSP GameData folder
3. Also download [Community Resource Pack][CRPRELEASES]. Download "Stable Release 112.0.1".
4. As with the USI collection, open the archive, then move the CommunityResourcePack folder from the GameData folder in the archive to the KSP GameData folder (overwriting the CommunityResourcePack that came with USI)
5. I recommend you install the [Bon Voyage][BonVoyageAddon] addon, it will be very useful for managing rovers later (it will save you hours of driving rovers around, crashing them, and having to reload a save game)

As for where to find the KSP GameData folder, it depends on your platform, and how you installed KSP. Check out the [KSP Wiki page on where to find the "root" directory][KSPROOTDIR] -- the GameData folder is inside that "root" directory (it's not actually called "root" that's just another name for the "top level" directory, which is likely called "Kerbal Space Program").

But ultimately you'll have the KSP GameData folder in front of you, along with the USI and CRP archives open, and all you need to do is copy those add-on folders across:

![The Kerbal Space Program GameData folder is open with the USI archive and the CRP archive open alongside. There are two arrows, the first is labelled 1 and points from the USI archive pointing at the GameData window, and a second arrow labelled 2, pointing from the CRP archive to the GameData window][AddOnInstallation]

### Pre-Packaged Save Game

If you want to use the tutorial ships, get the [WOLF Tutorial Save][MRWOLFTS] release file and unpack it now. Put put the **Ships** and **Subassemblies** folders into your save directory.

![The Kerbal Space Program saves directory showing the WOLF Tutorial save folder. Alongside that is the WOLF_Tutorial_Ships ZIP file contents. An arrow indicates that the contents of the ZIP file should be dragged directly to the WOLF Tutorial save folder][TutorialShipsInstall]

**Create a new sandbox game**. Configure the options as you see fit. I will typically turn off other launch sites, turn off missing crew respawning, and turn off stock vessels. This is just to keep things tidy and organised.

## WOLF Biomes

The foundation of industry in WOLF is the "WOLF Biome" and its associated depot. The basic idea is that each WOLF Biome has a certain abundance of resources, you dedicate a WOLF Biome to certain types of activity, and either transfer resources to other biome depots for further processing, or extract resources through WOLF "Hoppers" for use in the MKS industry that you're familiar with.

You can imagine WOLF Biomes as stuff that happens "behind the scenes" in the KSP world. You build up the industrial machinery to produce the goods that you need, hand that assembled factory to WOLF, then WOLF stops rendering those parts. The entire production line becomes an abstraction, with hundreds of parts abstracted away to a handful of numbers in the save game file.

Where the world of MKS is concerned with resource concentrations, extractor efficiency, engineer multipliers and storage capacity, the world of WOLF is concerned with resource abundance, expressed as one single number. Each WOLF biome has a certain abundance for each resource. There are no concentrations to worry about, nor are there survey maps to ponder and prime locations to target for resource extraction. There's just a number for each resource in each biome, which you can then directly feed into WOLF industry components.

The major catch with WOLF is that once you've committed to a certain production chain, there's no taking it back and making changes. With MKS infrastructure you can start producing Transport Credits then pivot to producing Material Kits and Specialised Parts by changing the recipes for a bunch of modules. With WOLF infrastructure, once you start producing something, that production chain will stay in place for the rest of your game.

### WOLF Route Builder Rover

As soon as you start the new sandbox game, head to the SPH and build yourself a survey rover. If you're using the tutorial ships, use the **WOLF Route Builder Rover** for this section. If you're building your own, you'll need the **Surface Scanning Module** from the stock game. Here's my **WOLF Route Builder Rover** which has a **Surface Scanning Module**, the **WOLF Transport Computer** which we'll discuss later, and the **Bon Voyage Autopilot** module (automatically incorporated into USI rover cabins) which I highly recommend (but more about that later).

![The WOLF Route Builder Rover rover with important components marked: surface scanner, transport computer and bon voyage autopilot][WolfDepotDeployerParts]

<!--

+ Place the rover further down the runway from the touchdown markings.
+ Open and pin the PAW for the command seat ("Malemute Cab") to the left
+ Open and pin the PAW for the WOLF Transport Computer to bottom right
+ Open and pin the PAW for the Surface Scanning Module to top right
+ Aim camera down with front of rover away from camera

-->

<!--
Label this image with:

1. Nuclear reactor and radiator (AG0)
2. Descent and flight core (AG9)
3. Surface operations core (AG8)
4. Surface Scanning Module
5. Bon Voyage controller
6. WOLF Transport Computer
7. Ladder (AG1)

Highlight:

1. "Bon Voyage Control Panel" action in cab PAW
2. "WOLF Biome" in scanner PAW
3. "Survey WOLF Biome" action in scanner PAW

-->

This rover has four side-mounted rocket engines which are useful for landing on small worlds like Minmus and Mun. They are not at all useful on Kerbin itself.

The life support on this rover can sustain one crew for about three years, or two crew for a little over 1 year. Crew is only necessary to increase the movement speed when controlled by Bon Voyage. Without crew, this rover will travel around 6m/s while with crew it will travel around 14m/s.

Action Groups:

- AG0: Turn the rover on and off. This affects all the components that produce or consume power such as the nuclear reactor, radiator, habitation and Nom-O-Matics, and lights.
- AG9: Switch control to Karibou Radial Probe for flight (the dome light will turn on to remind you that the rover is configured for flight)
- AG8: Switch control to probe core for driving (the dome light will come on to remind you that the rover is configured for driving)
- AG1: Extend/retract the ladder from the hitchhiker storage compartment

Important PAW features:

- **Bon Voyage Control Panel** in Malemute cab PAW
- **WOLF Biome** and **Survey WOLF Biome** in Surface Scanning Module PAW

### Surveying Harvestable Biome Resources

Launch this vessel and open the **Surface Scanning Module** PAW (Part Action Window, aka right-click menu). You'll see the usual MKS resource details in the Surface Scanning Module's window. For each resource there's a concentration tagged "[Surf]" (because it's a resource on the surface) which is then combined with harvester efficiency to determine how much of that resource you'll be extracting per second using MKS parts. WOLF doesn't use that data, so let's look at what data WOLF does use.

Now open the **WOLF Dashboard** and select the _Harvestable Resources_ pane. You'll see that it's empty right now. WOLF will populate this pane with details of resource abundance once the biome has been surveyed.

![WOLF Dashboard showing no biomes with harvestable resources][WolfDashboardHarvestableResourcesEmpty]

Looking back to the **Surface Scanning Module** PAW, there is one line under the MKS resources list specifying the "WOLF biome". You'll also see the "Survey WOLF Biome" action. Click it!

Recover this vessel.

## WOLF Dashboard -- Harvestable Resources and Depots

Now to check those resources. Switch scenes to the SPH and open the WOLF dashboard, then select the _Harvestable Resources_ pane:

![SPH scene showing WOLF Dashboard open to Harvestable Resources pane with KSC biome populated with harvestable resources][WolfDashboardHarvestableResourcesScannedBiome]

You'll have one Body/Biome option: Kerbin:KSC. There are four columns here which help you understand what resources you have access to:

1. Resource name, which represents the WOLF version of resources (as opposed to the "surface" resources)
2. Abundance, which is the WOLF equivalent to surface resource "concentration" (but it works completely differently)
3. Harvested, which is how much of the abundance you are currently extracting
4. Remaining, which is how much of the abundance is left to extract

The _Depots_ pane lists all your active WOLF Depots. Since you have no depots yet, it's empty.

![SPH scene showing WOLF Dashboard open to empty Depots pane][SPHWOLFEMPTY]

Now that the KSC WOLF Biome is surveyed, we need to deploy a WOLF depot. Before we do that though, have a quick look at the modules that make up the WOLF system, then we'll go over the rules of deploying them.

## WOLF Modules

To extract WOLF resources and convert them to useful outputs you'll use WOLF modules which are the WOLF equivalents to MKS systems such as mining drills, assembly lines, refineries and workshops.

From the SPH scene, start a new ship and open the _Planner_ pane in the **WOLF Dashboard**, and select the "WOLF" parts group in the selection pane on the left, then start planning this depot with a **WOLF Fabricator Module**. Set the **WOLF Fabricator Module** to produce _Material Kits_:

![SPH scene showing WOLF Dashboard open on Planning pane with a WOLF Fabricator Module as the first piece of the vessel under construction. The PAW shows Material Kits as the recipe.][SPHsceneFabricatorModuleWOLFDashboardPlanner]

There are two groups of values in the _Planning_ pane: the first is the _depot summary_ showing resources processed inside your WOLF Depot, the second is the harvestable resource report which shows the same details from the _Harvestable Resources_ pane but limited to those resources that you are actually harvesting with this depot. The _Planner_ now shows that you have a deficit of power, maintenance, technician crew point, chemicals, metals and polymers.

Add a _WOLF Maintenance Module_ and a _WOLF Power Module_. Now you'll see that you have surplus maintenance and power, but have incurred a deficit in various crew points. At this point, add a **Karibou Passenger Cabin** onto your WOLF modules to get 10 seats for crew and add an Engineer, Kolonist, Mechanic and Technician to your crew -- each crew member will add 10 crew points for their respective speciality. Add a probe core to the passenger cabin (I tend to use the _Avionics Package_ since it's small and cheap and provides all the necessary functionality). That's the crew points taken care of but now you have habitation and life support to worry about -- that's easily resolved by adding the **WOLF Habitation Module** and **WOLF Life Support Module**, leaving you with a deficit of food, oxygen and water (and the chemicals, metals and polymers for the fabricator).

Oxygen and water are available as _Harvestable Resources_ which means we can supply the depot with those resources using **WOLF MHU-550 Bulk Harvester** modules. Add two of those, configure one to harvest water and the other to harvest oxygen.

In the harvestable resource section of the planner you'll see that the harvesters are using 5 units each of the 1000 abundance of oxygen and 750 abundance of water, leaving 995 and 745 available. Note the numbers in the "Harvested" column: "0 (-5)" means that the KSC Biome Depot is currently harvesting 0 of that resource, and the craft that we are building will be harvesting 5 (thus reducing the abundance by 5).

Food is produced by an agricultural module or bioreactor module. Add a **WOLF Agriculture Module** and set it up to use the _Farm_ recipe. This has now added a demand for a farmer, dirt and fertiliser. Add a farmer to your crew, then you'll need three **WOLF MHU-550 Bulk Harvester** modules to get the dirt you need. To get fertiliser, we'll add a **WOLF MHU-550 Bulk Harvester** to harvest _gypsum_, then add two **WOLF Extractor Module** set to convert the _gypsum_ to _fertiliser_ (technically you only need one to feed the farm, but the harvester can feed two extractors). The two extractor modules have added a deficit for _Lab_ resource which is supplied by a **WOLF Science Module** so add one of those onto your growing pile of infrastructure, then add the scientist and medic crew that are needed for the science module.

Now add the **MHU-550 Bulk Harvesters** and **WOLF Refinery Modules** required for the chemicals (feed stock is minerals), metals (feed stock is metallic ore) and polymers (feed stock is substrates). These modules have added demand for a _Miner_ crew member so recruit one of those and add them to the crew module. To finish off this infrastructure install add another **WOLF Power Module**, and you should no longer have any deficits in the _Planner_.

You should now have this crew in the _Karibou Passenger Cabin_:

- Engineer
- Farmer
- Kolonist
- Mechanic
- Medic
- Miner
- Scientist
- Technician

**Note** that some of the _Material Kits_ produced by this infrastructure have immediately been consumed by other parts of the infrastructure (the habitation, life support and maintenance modules each consume 1 _Material Kits_ abundance). From the 5 _Material Kits_ produced by the fabricator, 3 have been consumed by the depot infrastructure leaving 2 for use elsewhere.

Before we can deploy this infrastructure we need to establish the depot itself. To do this, add a decoupler and a **WOLF Depot Module** with a probe core. Note that this depot module, probe core and decoupler combination is going to be used so often that I prepared a subassembly for it -- check Subassemblies for _Depot on Decoupler_. When you launch this craft you'll decouple the depot, which needs control in order to be useful.

What a beautiful creation! Did yours turn out like mine?

![SPH scene showing WOLF infrastructure required to support creation of 2 Material Kits abundance][SPHSCENE2MATKITS]

If you're familiar with the production chains from MKS you'll see that this WOLF infrastructure is a lot simpler than what is required in MKS, for example each **WOLF MHU-550 Bulk Harvester** is roughly equivalent to a mining ship with a logistics hub attached to the planetary warehouse -- each of those mining ships will be a dozen parts given the need for drills, ore tanks, radiators, power source, probe core and whatever else you normally put on your mining ships. That part count can severely bulk out your save file size, and slow your game to a crawl any time you load a production facility into physics range. WOLF removes all that complexity from the save file and physics simulation -- including the need to visit facilities every so often to update the resource processing chains.

### Establish KSC Depot

Launch that craft you just created. You're going to separate the depot and immediately hand it over to the WOLF system.

**Warning**: Any other parts attached to the WOLF modules will be consumed along with the WOLF modules when you hand them over to the biome depot, including any crew. In addition the WOLF Depot can not have any other WOLF components attached, _not even the Survey Scanner_.

Now that you have your **WOLF Depot Module** separated, it's time to establish your KSC Biome Depot:

![WOLF Depot Module with PAW showing "Establish Depot" action.][WOLFDEPOTPAWESTABLISH]

Just select the _Establish Depot_ action for the WOLF Depot Module, and the module will disappear. It belongs to WOLF now.

That depot has given us 1 Food, 1 Oxygen, 5 Material Kits, 5 Water, and 10 Power. This will significantly reduce the amount of infrastructure we need to get started — but remember that these bonus resources only apply to WOLF biomes on Kerbin.

Switch to the remaining depot infrastructure and connect it to the depot that you just established:

![Runway scene with 01 KSC Material Kits infrastructure showing PAW with 'Connect to depot' visible][RUNWAY01KSCMATKITSCONNECT]

Now open up the **WOLF Dashboard** to the _Depots_ pane to see the new production capacity from that WOLF infrastructure:

![Runway scene with WOLF Dashboard showing new production added][RUNWAYWOLFDASHNEWKSCDEPOTPRODUCTION]

### WOLF Infrastructure Expansion

**I highly recommend you get the Bon Voyage add-on**, it makes the process of deploying biome depots much, much easier.

To prepare for the next stage of the tutorial, let's expand the biome depots on Kerbin a little. For these first few expansions there are pre-built craft provided. For this part of the walkthrough we're focussing on the mechanics of surveying the biome, establishing the depot and then setting up a route for production to return to KSC. In the next section we'll work with the **WOLF Depot Planner** to build a depot to extract resources from the abundance presented by each depot.

The first task is to deploy basic depots. Start with the **WOLF Tutorial/Route Builder Rover** craft, add the **RBR Basic Depot** subassembly, then add an Engineer, a Kolonist and a Mechanic to the Karibou Passenger Cabin. Note: sometimes crewed components added using submodules or merged craft will not show up in the list of "parts with crew capacity". You can remedy this by removing the component and reattaching it.

Launch the rover, activate the parking brake to stop it rolling down the runway, then activate Action Group 10 (press "0" on the keyboard) to turn on the power supply.

Use the **Bon Voyage** autopilot to send the rover to _Kerbin Shores_ (0.0, -74.709). You can do this through the _Bon Voyage Control Panel_ option in the PAW for the **Malemute Cab** component of the rover. There is a list of locations like this later in this section, you might find it handy to keep a copy on hand. Activate the Bon Voyage autopilot (the "GO!" button) and then change scene to the Space Centre. Wait for the rover to reach its destination -- warp can help here -- and then switch back to the rover.

![The Bon Voyage Control Panel is accessed through the Malemute Cab PAW][RUNWAYDEPOTBONVOYAGE]

The process for establishing a depot using this rover is:

1. lock the brakes on
2. scan the WOLF biome with the **Surface Scanning Module**
3. decouple the depot module and establish the depot
4. undock the trailer and connect it to the depot

![Kerbin Shores scene with WOLF Depot Deployer - Depot and trailer are decoupled and Surface Scanner PAW is open. There are numbers 1, 2 and 3 indicating the order of operations.][KERBINSHORESDEPOTDEPLOYMENT]

Once you have completed those operations you should see the new depot established in the **WOLF Dashboard** with the Mechanic, Kolonist and Engineer resources added:

![Kerbin Shores scene with WOLF Dashboard open to Depots pane showing new Kerbin Shores depot][KERBINSHORESDEPOTDASHBOARD]

Now establish a WOLF Cargo route from the Grasslands back to KSC:

1. Open the **WOLF Transport Computer** PAW
2. Under _WOLF Cargo Transporter_  select _Connect to Origin Depot_
3. Use **Bon Voyage** to navigate to KSC at (-0.1, -74.647)
4. Open the **WOLF Transport Computer** PAW
5. Under _WOLF Cargo Transporter_ select _Connect to Destination Depot_

Repeat this process to deploy this simple infrastructure to Grasslands, Highlands and Mountains. These locations will help you find relatively flat ground in the right biome:

- Shores (0.107, -74.57)
- Grasslands (0.0 -75.38)
- Highlands (1.741, -77.339)
- Mountains (0.637, -78.659)

Remember you can return to KSC at (-0.1, -74.647). There are more biomes to explore but between KSC, Shores, Grasslands, Highlands and Mountains there are more than enough resources to complete this walkthrough.

Remember the basic process for establishing a new biome depot is:

- Prepare the WOLF Depot Deployer rover with the RBR Basic Depot subassembly
  - Required crew is Engineer, Kolonist, Mechanic (in the **Karibou Passenger Cabin**)
- On the runway, lock the brakes and start the reactor (AG0)
- Move the rover to the new biome
- Survey the WOLF Biome
- Decouple the **WOLF Depot** component
- Use the _Establish Depot_ action on the **WOLF Depot**
- Undock the **RBR Basic Depot** assembly
- Use the _Connect to depot_ action on the **RBR Basic Depot** assembly
- Switch vessels to the rover
- Use the _Connect to Origin Depot_ action on the **WOLF Transport Computer**
- Move the rover back to the KSC
- Use the _Connect to Destination Depot_ action on the **WOLF Transport Computer**
- Recover the rover

![Use the connect to origin depot action on the WOLF Transport Computer before departing the remote biome][ShoresDepotDeployerConnectOriginDepot]

![Use the connect to destinationi depot action on the WOLF Transport Computer after arriving at KSC][KSCDepotDeployerCoonectDestinationDepot]

If you want to know what's going on with the **WOLF Transport Computer**, check out the section on **WOLF Routes**. The executive summary is that you're setting up routes between depots over which you'll later be establishing resource transfers -- routes are like railways, transfers are the trains.

### Adding Production to WOLF Depots

The aim of our activities here is to establish an orbital ship yard and build spacecraft in orbit to further expand the WOLF infrastructure to other worlds. To build spacecraft at the orbital shipyard, you'll need _Material Kits_, _Specialized Parts_, _Alloys_, _Electronics_, _Prototypes_, _Robotics_ and _Synthetics_.

Let's start with the _Alloys_. In the SPH, load the **WOLF Route Builder Rover** and add an **RBR Trailer** subassembly. Open up the **WOLF Dashboard** to the _Planner_ pane and select _KSC_ Add a **WOLF Fabricator** module and change its recipe to _Alloys_. Now you have a deficit of _Rare Metals_, which are collected by a harvester module. Add a **WOLF MHU-500 Bulk Harvester** and set its recipe to _Rare Metals_. There's a deficit of _Rare Metals_ in this biome, so check through the remaining depots to see if you can find _Rare Metals_.

Unfortunately, it turns out that _Rare Metals_ are not a thing in Kerbin biomes. Okay, what about the others? _Electronics_ requires _Synthetics_ which in turn requires _ExoticMinerals_ ... which it turns out are not available on Kerbin either. Maybe _Prototypes_ then? No, they require _Electronics_ which we can't manufacture in WOLF on Kerbin. _Robotics_ are in the same boat, requiring _Alloys_. Last on the list are _Specialized Parts_ but it turns out that they require _Refined Exotics_ (refined from _Rare Metals_ and _Exotic Minerals_).

The only spaceship-building things we can make on Kerbin using WOLF infrastructure are _Material Kits_ and _Fuel_. What do we do about the rest? For the boot-strapping stage, any time we need _Specialized Parts_, _Alloys_, _Electronics_, _Prototypes_, _Robotics_ or _Synthetics_ the options are to buy them (create a new craft with a resource container full of the resource we're after), find some surface resources to extract and perform all the industry using MKS, or set up WOLF infrastructure where we _can_ find them and transport the supplies to the shipyard using WOLF routes and transfers.

For this walkthrough we're not going to go overboard with production, and as far as the other spaceship building materials go we'll simply buy them. Tens of abundance for _Material Kits_ and _Fuel_ will be enough to get us to Minmus where we'll find the resources that Kerbin doesn't have itself. Along the way we'll also produce _Fertilizer_, _Food_, _Oxygen_, and _Water_ to reduce the amount of infrastructure we need to establish on Minmus at the start.

### 01 Grasslands Material Kits

Clear the SPH build area and load up the **WOLF Route Builder Rover**, attach a **RBR Trailer** subassembly, then add the **RBR 5 Material Kits** subassembly to the trailer four times to get 20 _Material Kits_ production, put 3 x Miner and 3 x Technician in the **Karibou Passenger Cabin** (as indicated in the subassembly description), and check the _Planner_ pane of the **WOLF Dashboard** to see which biome will have the most resources left over after we commit to this _Material Kit_ production. For me this is the _Grasslands_ biome which had 100 _Minerals_ abundance before this infrastructure took 20 away.

The _Planner_ shows that there's a deficit of Power and Maintenance, so add a **WOLF Maintenance Module** and a **WOLF Power Module** to the trailer and you should have a completed depot expansion.

Launch the rover and send it to the _Grasslands_ biome (0.0 -75.38).

Here's what the **WOLF Route Builder Rover** with 4 x **RBR 5 Material Kits** subassemblies and the required crew should look when you're ready to launch:

![SPH scene with Route Builder rover and attached Material Kits subassemblies][SPHDDRMaterialKitsAndCrew]

As is usual with the Depot Deployer Rover:

- move the rover to the destination biome
- undock the trailer and connect that to the depot
- connect the transport computer to the "origin" depot
- send the rover back to KSC
- connect the transport computer to the "destination" depot
- recover the vessel

The _Grasslands_ depot will eventually be expanded to produce 115 _Material Kits_.

This depot expansion is available in the Walkthrough game as **01 Grasslands Material Kits** under the **WOLF Depot Deployers** folder in the SPH.

Crew:

- 3 x Miner
- 3 x Technician

### 02 Shores Fuel and Life Support

With that _Material Kit_ production established, send a Depot Deployer rover with the **RBR Fuel and Life Support** subassembly to the Shores biome.

Crew:

- Farmer
- 2 x Geologist
- Medic
- Scientist

After those depot expansions the _Depots_ tab of your **WOLF Dashboard** should look something like this:

![SPH scene with WOLF Dashboard showing material kits and fuel production from KSC, Shores, Grasslands, Highlands and Mountians][SPHWOLFDASHSTARTERPRODUCTION]

## WOLF Routes

It's all well and good having that _Material Kits_ production chain set up in the mountains, but what do we do with the output? At present all of this work has set up _abundance_ of certain resource types in the invisible world of WOLF. Eventually you'll pull resources out of WOLF into the MKS world.

The next step on the way from WOLF production to MKS extraction is getting those WOLF resources to orbit, where we want to use Material Kits and other resources to build spaceships. The immediate progress we need to make is _transferring__ the resources from the WOLF depots to the KSC and then _transferring_ them to orbit over WOLF _routes_.

WOLF handles transport of resources from one biome to another by way of _routes_ which are paths established for _transfers_ to move over -- conceptually, routes are a railway and transfers are the regular trains on that railway. You establish a route by travelling between biomes using the **WOLF Transport Computer** to connect origin and destination depots, with the capacity of the route determined by the **WOLF Cargo Kontainers** attached to the rover. Moving a vehicle between origin and destination depots with the transport computer tracking the trip will add _Route_ between the source biome and the destination biome with a certain _cargo space_.

You already have some routes established as part of the initial deployment of WOLF depots with the WOLF Depot Deployer, here's what they look like in the _Routes_ pane of the **WOLF Dashboard**:

![SPH scene with WOLF Dashboard showing the Routes pane][SPHWOLFDASHROUTESPANE]

This panel is showing us that there are routes between specific origin and destination biomes that have a certain capacity in units of _Cargo Space_. You can then create _Transfers_ on that route, which will move abundance of a resource from one biome depot to another.

### WOLF Transfers

In this walkthrough the main purpose of setting up these biomes is to get Material Kits and Fuel to orbit to start building spaceships. To get the food, fuel and material kits from the various biome depots to orbit, first we need to get them to the launch site. This means setting up resource transfers over the established routes. To establish a resource transfer open the **WOLF Dashboard** to the _Routes_ pane. Select the _Manage Transfers_ button which will show you the _Manage Transfers_ interface:

![SPH scene with WOLF Dashboard showing the Manage Transfers interface][SPHWOLFDASHMANAGETRANSFERS]

This dialog is use to set up resource transfers over a route. The numbers visible in this dialog show:

- The resources and their abundance at the source biome depot
- The selected resource
- The abundance of that resource in the source biome depot
- The current available/incoming values of the resource in the destination biome
- The list of resources that you have already selected for transfer on this route
- How much payload capacity is left for transfers
- How much payload capacity has already been used

How much of a resource you can add to transfers on this route is the smaller number of the abundance of the resource or the available payload. In the example above there are 20 Material Kit points available, and the payload of 45 has space for all of them with room to spare.

When you request a new transfer you'll allocate an _abundance_ of resource to a transfer, then the _abundance_ of that resource will be reduced in the source biome and increased in the target biome, and the route will have a new _Transfer_ using up some of its capacity.

To transfer resources select the resource in the top pane, enter the abundance you wish to shift between depots in _Transfer Amount_ then select _Transfer_. Do that now to move 5 Material Kits from the Grasslands depot to the KSC depot:

1. Open the **WOLF Dashboard** to the _Routes_ pane
2. Click _Manage Transfers_  to open the _Transfer Resources_ interface from the _Routes_ pane of the **WOLF Dashboard**
3. Select "Kerbin:Grasslands => Kerbin:KSC" from the dropdown at the top (the left/right arrows will help when your list is too long to fit on the screen)
4. In the list of resources, select the down-pointing triangle next to _MaterialKits_
5. Set _Transfer Amount_ to 20
6. Click _Transfer_
7. You should see the lower pane update with the new transfer of 20 _MaterialKits_ over this route
8. The Origin abundance will drop by 20
9. The Destination abundance will rise by 20
10. The Available Payload will drop by 20
11. _Close_ the _Transfer Resources_ window

Here's the _Transfer Resources_ window with the new transfer set up over the Grasslands to KSC route:

![KSC scene with Transfer Resources interface showing a new transfer of 6 MaterialKits from Grasslands to KSC][KSCTransferMaterialKitsGrasslandsToKSC]

Now click the "X" next to that 6 Material Kits transfer in the lower pane, and the abundance in the source and destination depots will be restored along with the available payload.

Now set up the Material Kits transfer to move:

- 20 Material Kits from the Grasslands depot to the KSC depot
- 10 Food from the Shores depot to the KSC depot
- 35 Fuel from the Shores depot to the KSC depot
- 10 Oxygen from the Shores depot to the KSC depot
- 10 Water from the Shores depot to the KSC depot

Close the _Transfer Resources_ window.

The _Routes_ pane of the **WOLF Dashboard** will now show the resources being transferred between the various biomes and the KSC. Here's what my transport routes look like with the depots transferring some resources to KSC:

![KSC scene with WOLF Dashboard showing transfers from highlands, mountains and shores to KSC][KSCTransfersFromHighlandsMountainsShores]

If you have more Material Kit, fuel, water and food abundance than will fit in the payload, you can simply connect the route more times with your route-building vehicles to increase the payload size.

The small portions of abundance that we have produced and transferred will be adequate for the next stages of the walkthrough. Feel free to expand your depots by adding more production modules, adding more payload capacity to the routes using the route builder rover, and transferring the extra abundance to KSC.

### Transport Routes and Transport Credits Costs

Up till now we've kept the transport routes simple by only connecting biomes that can be reached with electric rovers. It's time to kick it up a notch and learn about Transport Credits, which is an abstraction of the process of building launch vehicles, fuelling them and launching payloads to orbit (or deorbiting payloads to bring them to the surface). Transport Credits also represent an abstraction of building and fuelling tugs and freighters that operate between worlds -- basically any transfer that involves the consumption of stuff (rocket stages, propellant, etc) is abstracted to Transport Credits.

The first thing we'll do here is a few test flights to understand how many _Transport Credits_ we'll need for sending supplies to orbit (or roughly, how Transport Credits correlate to delta-v and ship size), and then we'll have a look at an optimisation that will reduce Transport Credit cost to 0. Let's start with a small rocket, a medium sized rocket, a 3t payload SSTO spaceplane, and a 55t payload SSTO spaceplane. With enough Transport Credits each flight will add a certain payload capacity to the available routes from KSC to Kerbin Orbit, with the payload capacity being determined by the _WOLF Cargo Kontainers_ on each launch vehicle. We'll get the gory details soon!

### Quick and Dirty Transport Credit Example Flights

**Save your game here**, give it a name like "Before Transport Credits". Skip ahead to the next section (_Extracting Resources from WOLF to MKS_) if you don't want to learn about transport costs and how to avoid them. You're going to be restoring to this point after experimenting with _Transport Credits_, and through the rest of the walkthrough there will be no transport costs other than the time it takes to set them up.

In the VAB, put together a rocket that can carry a single 3t **2.5m WOLF Cargo Kontainer** to orbit using 2.5m parts. The **WOLF Tutorial 2.5m SSTO** contains:

- 2.5m WOLF Cargo Kontainer
- RC-001S Remote Guidance Unit
- Protective Rocket Nosecone Mk7
- Rockomax Jumbo-64 Fuel Tank
- RE-I5 "Skipper" Liquid Fuel Engine
- WOLF Transport Computer

Send that to the launch pad, select the _Connect to Origin Depot_ action on the **WOLF Transport Computer** under the _WOLF Cargo Transporter_ heading, and launch the rocket to a 80km orbit.

![Connect the WOLF Transport Computer to the origin depot before launch][SmallSSTORocketStartRouteAtLaunch]

Once in orbit, check the "Route cost" reported by the **WOLF Transport Computer**.

If you try to use the **Connect to Destination Depot** action, you should get an error message about needing more Transport Credits to complete that operation. Revert to launch, and run it a few times just to see that the "Route cost" is predictable. My flights came up with a route cost of 30 _Transport Credits_ which works out to a _Credits/Payload_ cost of 10.

![Sample flight of 2.5m rocket showing a route cost of 30][SmallSSTORocketRouteCost30]

Revert to vehicle assembly and do the same thing with a 3.75m rocket. The _WOLF Tutorial 3.75m SSTO_ is roughly:

- 2 x 3.75m WOLF Cargo Kontainer
- Protective Rocket Nosecone Mk7
- RC-L01 Remote Guidance Unit
- Advanced Reaction Wheel Module, Large
- WOLF Transport Computer
- Kerbodyne S3-14400 Tank
- S3 KS-24x4 "Mammoth" Liquid Fuel Engine

Send that to the launch pad, select the "connect to origin depot" on the WOLF Transport Computer, and launch the rocket to an 80km orbit. As before, check the "route cost", revert to launch and run the process again to show that the "route cost" is predictable. My flights came up with a route cost of 80-ish, giving a _Transport Credit Per Unit_ cost of around 6. Revert to vehicle assembly when done.

![Sample flight of 3.75m rocket showing a route cost of over 80][KERB375ROCKETCREDITS]

Now do the same thing with spaceplanes. The two I use are the **WOLF SSTO** and the [ES-96 Python by Juggernoob](https://steamcommunity.com/sharedfiles/filedetails/?id=1722161481) which I find to be aesthetically pleasing and easy-to-fly SSTO spaceplanes.

**Instructions:** for both these spaceplanes the procedure to get to orbit is:

- set throttle to maximum
- turn SAS on to stability assist
- stage once to light the engines
- rotate off the runway to 10 degrees at about 140m/s and immediately retract landing gear
- hold the nose at 10 degrees for the whole flight through the atmosphere
- when the airbreathing mode is insufficient to keep accelerating, switch to closed cycle (Action Group 1)
- push the apoapsis to 80km and cut the throttle
- cruise to the top of the atmosphere, plot a circularisation burn at apoapsis
- execute that burn.

My flights with **WOLF SSTO** ended up producing routes with a cost of 9 for 3t cargo, or about 3 credits/unit.

![Sample flight of WOLF SSTO showing route cost of 8 for 3t cargo][SSTORTCOST8]

The **ES-96 Python** got to orbit in the order of 80 to 90 Credits for 42t. The **WOLF ES-96 Python** in the tutorial ships package has already been modified and will automatically start the transport route when you stage to launch (the **Transport Computer** is in the cargo bay with the _Connect to origin depot_ action linked to the _stage_ action group).

![Sample flight of WOLF ES-96 PYTHON showing route cost of over 80 for 42t][ES96RTCOST85]

### Transport Module for Transport Credits

How do we produce Transport Credits? The short version is that _Transport Credits_ are produced by the _WOLF Transport Module_. By now you should be familiar with the drill: start assembling a new WOLF infrastructure component with the WOLF Dashboard open to the Planning pane, beginning with the WOLF Transport Module. Fuel is produced by the Fuel(Ore) or Fuel(H2O) recipes in the WOLF Refinery Module — each recipe will take 5 points of input availability and provide 2 points of Fuel availability. As usual one harvester will provide sufficient Ore or Water for two refineries.

The "atomic" component of a Transport Credit production line is 1 Transport Module (producing 10 _Transport Credits_ from 10 _Fuel_), 3 MHU-500 harvesters (_Water_), and 6 Refinery Modules (producing 2 _Fuel_ from 5 _Water_) this needs to be supplemented with 1 abundance of _Material Kits_. To produce the target of 100 Transport Credits to get our _Fuel_ and _Material Kits_ to orbit we need to start off with:

- 10 x WOLF Transport Module
- 30 x MHU-500 harvesters (harvesting water)
- 60 x WOLF Refinery Module (producing fuel from water)
- local or imported abundance of 10 x Material Kits

Then you add all the habitation, power, maintenance and other infrastructure required to support this.

![VAB showing the ridiculous WOLF infrastructure required to produce 100 transport credits][VABWOLFTutorial100TransportCredits]

One catch with _Transport Credits_ is that you can't deliver them elsewhere: they can only support the establishment of routes from the biome which they're produced in. Thus to use _Transport Credits_ to fund transfers from KSC to Kerbin Orbit, you need to deploy this infrastructure at KSC.

### How To Avoid Transport Credit Costs of Propellant-Consuming Vehicles

Now that you've gone to the effort of figuring out that Transport Credit infrastructure, I have a secret to share: you can make the system work to your advantage and completely eliminate the Transport Credit cost of these route-building flights.

How? Put a propellant depot in orbit, fly your transport vehicle to that depot and refuel before connecting the **WOLF Transport Computer** to the destination depot. You can also accomplish the same thing by putting an empty fuel tank near the launch site and transferring all the fuel out of your craft before starting the route (then refuelling before you launch). Because the transport cost is calculated based on the difference in mass between the start and the end of the transport route, if you can restore all the consumed mass you can get a transport route that costs 0 _Transport Credits_. This is how you'd do it if you had an established MKS or stock infrastructure (for example exporting propellant from Minmus to Kerbin orbit), flying your freighter to the destination and refuelling to get it back to the origin port.

Here's the **WOLF SSTO** at the end of a 3t haul to orbit having just refuelled. How many transport credits to fly 3t to orbit? 0. Let's make this work for you!

![WOLF SSTO in Kerbin orbit with Kerbin Shipyard in background and WOLF Transport Computer action window showing route cost 0 and route payload 3][WOLFSSTO0CREDITS]

**Go back and load your "Before Transport Credits" save game**.

## Bootstrapping Kerbin Orbit WOLF Infrastructure

Load the **WOLF Shipyard Launcher** that you'll find in the VAB from the tutorial ships package, under the **WOLF Tutorial Shipyard** folder. Launch that shipyard to an 80km orbit, undock the **WOLF Depot** component and establish the orbital depot.

Now to expand on this shipyard to provide a propellant supply and the ability to construct spacecraft for the expansion to Minmus and Mun. To start with, let's add a propellant supply to the shipyard. To accomplish this:

- build a route to provide WOLF MaterialKits that the shipyard
- supply the MKS resources (other than Material Kits) required to build the _Fuel Hopper_ shipyard component
- supply the 4000 Material Kits required to deploy the shipyard

The WOLF ES-96 Python will need around 15,000 fuel and oxidizer to replenish at the end of its run. One option is to send up a large tanker with the required propellant. Check out the **Shipyard Bootstrap** vessel under the **WOLF Tutorial Shipyard** folder. This will bootstrap the Kerbin Shipyard, and allow you to establish a route from KSC to Orbit:

1. From SPH launch the **KSC Passenger Terminal** and park it near the eastern end of the runway
1. Launch the **WOLF ES-96 Python**
1. Transfer all the propellant from the **WOLF ES-96 Python** to the **KSC Passenger Termianl** (the forklift icon on the toolbar)
1. Start the cargo route
1. Refuel the **WOLF ES-96 Python** from the **KSC Passenger Terminal**
1. Fly the **WOLF ES-96 Python** to orbit
1. Connect the cargo route to orbit (this should require 0 transport credits)
1. Rendezvous with the **KSC Shipyard**
1. Transfer all propellant from **WOLF ES-96 Python** to **KSC Shipyard**
1. Start the cargo route
1. Refuel the **WOLF ES-96 Python** from **KSC Shipyard** (you should only need 600m/s)
1. Return WOLF ES-96 Python to KSC
1. Connect the cargo route to KSC

The shipyard will also need advanced MKS materials which we are not producing yet. As you might expect, there's already a craft available to deliver the advanced construction materials that will be required. Look at the **Advanced Materials Delivery** craft, which will deliver the following in about the proportions required:

- Specialized Parts
- Alloys
- Synthetics
- Robotics
- Electronics

One of these will bootstrap the Kerbin shipyard, then a second will bootstrap the Minmus shipyard later. After that all the resources will be produced through WOLF infrastructure and expansion to other worlds becomes much easier. For the immediate mission:

1. Launch the **Advanced Materials Delivery** rocket
2. Rendezvous **Advanced Materials Delivery** with **Kerbin Shipyard**
3. Dock **Advanced Materials Delivery** to **Kerbin Shipyard**

With all that work taken care of, it's time to commission the shipyard!

### Commission Kerbin Shipyard

To commission the Kerbin Shipyard, you need to complete these tasks:

1. Transfer Material Kits and Fuel from KSC depot to Kerbin Orbit depot
2. Connect the Material Kit hoppers on the shipyard to the depot
3. Build the **Fuel Hopper** expansion for the shipyard
4. Connect the **Fuel Hopper** to the depot

With the propellant handling in place, you can rendezvous further route-building craft with this shipyard to refuel (for example the **WOLF SSTO** or **WOLF ES-96 Python**), and start building your orbital industry from there.

 ![WOLF ES-96 Python in Kerbin orbit with just-launched Kerbin Shipyard in background, WOLF Transport Computer action windows showing route cost 0]()

Keep expanding the route between KSC and Kerbin Orbit to 80 units. Two flights of the **WOLF ES-96 Python** should be plenty:

- 20 fuel
- 20 material kits
- 10 water
- 10 oxygen
- 10 food

As you did the last time when setting up transfers over a route:

1. Open the **WOLF Dashboard** to the _Routes_ pane
2. Click _Manage Transfers_  to open the _Transfer Resources_ interface from the _Routes_ pane of the **WOLF Dashboard**
3. Select "Kerbin:KSC => Kerbin:Orbit" from the dropdown at the top (the left/right arrows will help when your list is too long to fit on the screen)
4. In the list of resources, select the down-pointing triangle next to _MaterialKits_
5. Set _Transfer Amount_ to 20
6. Click _Transfer_
7. You should see the lower pane update with the new transfer of 20 _MaterialKits_ over this route
8. Repeat steps 4-6 for fuel, water, oxygen and food
9. _Close_ the _Transfer Resources_ window

![WOLF Dashboard open to the Routes pane. Transfer Resources dialog is open, showing a transfer of material kits and fuel from the KSC depot to the Kerbin Orbit depot][KERBYARDTRANSFERS]

With those transfers organised, it's time to extract the WOLF resources into the MKS industry system. This is done using the various hoppers on the Kerbin Shipyard.

## Extracting Resources from WOLF to MKS

Now open the **WOLF Dashboard** to the _Depots_ pane, expand the _Kerbin: Orbit_ depot so you can watch the figures while we configure the hopper modules, and set the hopper up:

 1. Open a _Material Kits_ Manufacturing Hopper's PAW (for this we want the PAW and the WOLF Dashboard open)
 2. Click _Connect to depot_
 3. Click _Start hopper_

Observe that the abundance of a resource will be reduced the moment you connect the hopper to the depot, regardless of whether or not the hopper is running. Here's what it should look like for you now:

![At the shipyard in orbit, WOLF Dashboard is open to the Depots pane and the Kerbin: Orbit depot is expanded to show the incoming/outgoing/available resources. There are Material Kits outgoing to service the connected manufacturing hopper. The PAW for the manufacturing hopper is open showing the "Disconnect from depot" and "Stop hopper" buttons.][KERBYARDMATKITHOPPERSTART]

While you are here, keep the **WOLF Dashboard** open and see what happens when you stop the hopper and disconnect it from the depot. What you should see happen is that the local resource production will stop when you stop the hopper, and the abundance of the resource in the Kerbin Orbit depot of the **WOLF Dashboard** _Depots_ pane will be deducted from _Outgoing_ and added to _Available_. When you're ready, reconnect the hopper and start it up again.

Now connect and start the other _Material Kits_ hoppers. The combined output of three 3.75m Manufacturing Hoppers will be 15,000 _Material Kits_ a day. We'll need 38,782 for the next step. The fourth hopper is configured for Specialized Parts, which are not available yet.

### Establishing the Kerbin Shipyard

Now that resources are flowing to the shipyard, wait until there are 39,000 _Material Kits_ available. With those resources you can deploy the **KS-250-O KonStructor** module (using the _Deposit Resources_ PAW action) and build a _Fuel Hopper_ which you will find in the _WOLF Tutorial Shipyard_ folder:

1. Open the Konstructor's PAW (right-click menu)
2. Select _Open Konstructor_
3. From the _Konstructor_ window select _Select a ship_
4. From the vessel selection dialog open the _WOLF Tutorial Shipyard_ folder and select _Fuel Hopper_
5. Verify that you have all the materials required to build the _Fuel Hopper_
6. Select _Build_
7. After a brief delay the _Fuel Hopper_ will pop into existence and control will be transferred to the new vessel
8. Transfer monopropellant from _Kerbin Shipyard_ to the _Fuel Hopper_ using the MKS _Transfer Resources_ window (forklift icon)
9. Dock the _Fuel Hopper_ with the ship yard. The red/green navigation markers are mounted "forward" of the Clamp-O-Tron Sr to help you orient the vessels neatly
10. Open the PAW on one of the WOLF Fuel Hopper modules
11. Click _Connect to depot_
12. Click _Start hopper_

As with the _Material Kits_ in the manufacturing hoppers, you should see the depot's abundance of fuel drop by 5 to service this hopper. Each Manufacturing Hopper configured for Material Kits will produce 5000 Material Kits per day.

Connect the remaining Fuel Hopper modules to the depot and start them. Each Fuel Hopper configured for LF/Ox will produce 450 LF/day and 500 Ox/day.

To prepare for the Minmus expansion, add an **A/E/R/S Hopper** shipyard component to the **Kerbin Shipyard**.

Here's a finished Kerbin Shipyard, ready to start the next phase of expansion:

![Assembled Kerbin Shipyard showing shipyard component and fuel hopper docked in orbit][KERBYARDCOMPLETE]

### Crew Transport Preparation

- Add a **Passenger Terminal** to **Kerbin Shipyard**
- Build **Crew Transport** and move it to a parking orbit
- Launch **Reactor Maintenance** to rendezvous with **Crew Transport**
- Dock **Reactor Maintenance** to **Crew Transport**
- Perform Maintenance on **Crew Transport** nuclear reactor (engineer needs to do an EVA)
- Put **Reactor Maintenance** into a parking orbit
- At some point in the future, add a **Passenger Quarters** module to **Kerbin Shipyard** which will be used to refresh hab timers for Kerbals in orbit (eg: the engineer aboard **Reactor Maintenance**)

For the duration of the Minmus campaign, the passenger terminal at **Kerbin Shipyard** will be used as a layover for crews launched from Kerbin waiting for the **Crew Transport** to arrive.

## Minmus Expansion

To establish the Minmus shipyard the basic steps are:

1. Build an **Expansion Shipyard**, launch it to Minmus, place it in a 20km circular orbit
2. Launch a new **Advanced Materials Delivery** rocket and send it to Minmus to dock with the shipyard
3. Build the **Orbital Route Builder 75** and establish a cargo route between Kerbin Orbit and Minmus Orbit
4. Use the route builder to establish cargo route between Minmus Orbit and Minmus Greater Flats
5. Use the route builder to establish cargo routes between Greater Flats and the other depots on Minmus

Let's go through that now. If this list has enough detail for you, work through it and skip to the section **Minmus Expansion**.

### Minmus Shipyard

The **Expansion Shipyard** requires approximately the following materials:

- 137,000 Material Kits
- 966 Specialized Parts
- 266 Alloys
- 533 Synthetics
- 63 Robotics

There are sufficient advanced materials remaining from the original delivery, so you'll just have to wait the 10 days for the required quantity of Material Kits to arrive. It will take about 16 days to produce the propellant required for the Expansion Shipyard too. You can speed this up by adding another _Fuel Hopper_ and _Manufacturing Hopper_ assembly to the **Kerbin Shipyard** along with the necessary Kerbin-based production, routes and transfers. For the purpose of the walkthrough, just "warp to next sunrise" 16 times to produce the required material kits and propellant.

Once you have the materials, build the **Expansion Shipyard**, fill it with propellant and send it to **Minmus**.

When the **Expansion Shipyard** arrives at **Minmus**:

- Place the **Expansion Shipyard** in a 20km circular orbit
- Undock the _Depot_ module at the front (it's attached via the Clampotron)
- Switch to the _Depot_ spacecraft
- Select _Establish Depot_ from the depot module's PAW
- Switch back to the **Expansion Shipyard**
- Rename the **Expansion Shipyard** to **Minmus Shipyard** if you haven't already

Now the advanced materials at **Kerbin Shipyard** will be running low, so launch a second **Advanced Materials Delivery** to top it up.

Launch a third **Advanced Materials Delivery** craft and send it to Minmus to rendezvous and dock with the **Minmus Shipyard**. Immediately build a **A/E/R/S Hopper** and dock it to **Minmus Shipyard**.

Now return to the **Kerbin Shipyard** and build the **Orbital Route Builder 75**. The **Orbital Route Builder 75** requires 31335 _Material Kits_ (2 days production) and 6480 _Liquid Fuel_ (4 days production).

- Start a cargo route and send the **Orbital Route Builder 75** to **Minmus**
- At **Minmus**, rendezvous the **Orbital Route Builder 75** with **Minmus Shipyard**
- Refuel and complete the route
- Disconnect all the hoppers at **Kerbin Shipyard**
- Transfer these resources from _Kerbin Orbit_ to _Minmus Orbit_
  - 20 fuel
  - 15 material kits
  - 10 water
  - 10 oxygen
  - 10 food
- Start a cargo route and send the **Orbital Route Builder 75** back to **Kerbin Shipyard**

The **Orbital Route Builder 75** should be sent back and forth a few times to build up around 80 units of route capacity in each direction. This is to cater for some materials that we will be sending to Minmus to bootstrap the infrastructure, and then to cater for resources returning to Kerbin from Minmus as Minmus industry is established.

With 15 Material Kits abundance from Kerbin, **Minmus Shipyard** will be producing 15,000 _Material Kits_ per day. When there are 4,000 _Material Kits_ available, ,deploy the _Konstructor_.

Now **Minmus Shipyard** has been established, it's time to expand our WOLF infrastructure to **Minmus** itself.

### Minmus Overview

At this point you should be familiar with:

- Establishing WOLF biome depots
- Establishing routes between WOLF biome depots using a rover
- Configuring resources transfers over routes
- Configuring WOLF resource hoppers to convert WOLF resources to MKS resources

What comes next is learning how to wrangle the armies of Kerbals that will be required to operate the WOLF infrastructure on Minmus. But first, let's find what resources are available on Minmus.

Some things to consider for Minmus: first is that the expansion will be strapped for resources. After this infrastructure is in place we'll have the resources required to bootstrap a new world without any stress. For Minmus we're starting with a fixed amount of resources from one shipment and boot-strapping the infrastructure to support a shipyard.

Secondly, I've found Minmus hostile to rovers. My rovers will slide forever while a regular lander sits a little awkwardly on a slope. There are currently issues with the wheels on the USI rovers (Malemute and Karibou) so you can't manually drive them anywhere, and the same slipping and sliding issues affect them anyway.

What I have found easiest for Minmus is using rockets to drop depot expansions onto the surface from orbit. We'll also be shipping crew in from Kerbin, since WOLF requires a significant investment in infrastructure to transport crew (we'll get to that for the Mun expansion).

Resource production required to supply **Minmus Shipyard** will be the minimum required to run 3 x 3.75m _Material Kits_ hoppers and 1 x 3.75m hopper of each remaining building material excluding Prototypes. Here's a summary list, pardon my shorthand in the brackets. The shorthand "Chemicals x 25 (1 x 25)" means "we need 25 chemicals to support Material Kits, which is 1 per Material Kit abundance, and we're producing 25 abundance of Material Kits."

1. Material Kits x 25 (15 for station + 5 for electronics + 5 for robotics)
   - Chemicals x 25 (1 x 25)
   - Metals x 50 (2 x 25)
   - Polymers x 50 (2 x 25)
2. Specialized Parts x 5
   - Refined Exotics x 10 (2 x 5)
     - Exotic Minerals x 20 (2 x 2 x 5)
     - Rare Metals x 30 (3 x 2 x 5)
   - Silicon x 15 (3 x 5)
3. Alloys x 6 (1 for station + 5 for Robotics)
   - Metals x 6 (1 x 6)
   - Rare Metals x 24 (4 x 6)
4. Synthetics x 6 (1 + 5 for Electronics)
   - Exotic Minerals x 24 (4 x 6)
   - Polymers x 6 (1 x 6)
5. Electronics x 1
   - Material Kits x 5
   - Synthetics x 5
6. Robotics x 1
   - Alloys x 5
   - Material Kits x 5

The sum total thus becomes:

- Chemicals x 25 (only for MK)
- Exotic Minerals x 44 (20 for SP + 24 for Synthetics)
- Metals x 56 (50 for MK + 6 for Alloys)
- Polymers x 56 (50 for MK + 6 for Synthetics)
- Rare Metals x 54 (30 SP + 24 for Alloys)
- Silicon x 15 (only for SP)

Because of the proportions in which the various materials are consumed, this setup will be enough to support production of the advanced materials up until around the point we have a hundred or so Material Kits hoppers. While it could be possible to transport these resources around the place using freighters, in this walkthrough we're pursuing the goal of making each shipyard independent. The extra work required is actually fairly low.

Production of _Prototypes_ is beyond the scope of this walkthrough. Each unit of _Prototypes_ requires 5 x _Electronics_, 5 x _Robotics_, and 5 x _Specialized Parts_. Working backwards:

- Prototypes x 1
  - Electronics x 5
    - Material Kits x 25 (5 x 5)
    - Synthetics x 25 (5 x 5)
      - Exotic Minerals x 100 (4 x 25)
      - Polymers x 25 (1 x 25)
  - Robotics x 5
    - Material Kits x 25 (5 x 5)
    - Alloys x 25 (5 x 5)
      - Rare Metals x 100 (4 x 25)
      - Metals x 25 (1 x 25)
  - Specialized Parts x 5

Later we'll look at producing _Colony Supplies_ at KSC:

1. Colony Supplies x 5 (1 fabricator)
   1. Machinery x 5 (1 fabricator)
      1. MaterialKits x 3
      2. Specialized Parts x 2
   2. MaterialKits x 3
   3. Specialized Parts x 2

This amounts to 6 _material Kits_ and 4 _Specialized Parts_ per batch of 5 _Colony Supplies_. So while we're establishing industry on Minmus, keep an eye out for the extra resources required to produce _Colony Supplies_.

### Minmus CommNet and Skycrane

- Build **Satellite Bundle** and deploy the relay sats
  - Deployer should go to 357.941km x 534.657km orbit
  - Release one relay satellite just before each periapsis
  - Circularise each relay satellite at periapsis (357.941km circular orbit, 40400s / 1d 5h 13m 20s period, aka 1 Minmus day)
  - Double-check the deployer's orbit between deployments
  - When three relays are deployed, put the deployer into a 200km polar orbit
  - Deploy the scanner and perform an orbital analysis
- Build the **Skycrane** (WOLF Depot Landers)

For the _Greater Flats_ and _Midlands_ biomes on **Minmus**:

- Build a **Skycrane Depot Box**
- Rendezvous **Skycrane** with the **Skycrane Depot Box**
- Dock the **Skycrane Depot Box** with the **Skycrane**
- Land the **Skycrane** at the new biome
- Survey the WOLF biome
- Undock the Depot Box
- Switch to the Depot Box
- Select "Establish depot" from the Depot module's PAW
- Return Skycrane to parking orbit

The remaining biome depots must wait until the Minmus Shipyard is self-sufficient.

Useful Minmus landing sites:

- Midlands (4.390, -86.594 or 4N 86 43'37"W -- flat plateau to the immediate east of Great Flats)
- Greater Flats (0, -7.5 or 0 7 30'00"W)
- Flats (1.5, -40 or 1 30' 0"N 40 0' 0"W -- bottom lobe of the flats just NW of Greater Flats)
- Lesser Flats (9.404, -178.003)
- Great Flats (-10, -92 or 10S 92W)
- Poles (78.045, 164.276) (exotic metals, minerals)
- Lowlands (0.026, -51.516)
- Highlands

### Minmus Route Preparation

By now you should have completed two cargo routes from _Kerbin Orbit_ to _Minmus Orbit_ and back. Use **Orbital Route Builder 75** to build a route from **Minmus Shipyard** to _Greater Flats_ on **Minmus** and back, and from _Greater Flats_ to _Midlands_ and back:

- Rendezvous **Orbital Route Builder 75** with **Minmus Shipyard**
- Move all the propellant from the route builder to the shipyard
- Start the route
- Put enough propellant in the route builder to give ~500m/s delta-v
- Land **Orbital Route Builder 75** on _Greater Flats_
- Complete the route (which should be 0 cost)
- Start a new route
- Launch the route builder and rendezvous with **Minmus Shipyard**
- Refuel the route builder
- Complete the route (which should be 0 cost)

Now build the **Skycrane Propellant Dump** and deliver it to _Greater Flats_ using the **Skycrane**. You don't need to put any propellant in it.

With the **Orbital Route Builder 75**:

- Rendezvous with **Minmus Shipyard**
- Transfer all propellant to the shipyard
- Start a new route
- Fully load the **Orbital Route Builder 75** with propellant
- Land at _Greater Flats_ within 200m of the **Skycrane Propellant Dump**
- Complete the route (_Minmus Orbit_ to _Greater Flats_, should be 0 cost)
- Transfer all propellant to the propellant dump
- Start a new route
- Load about 800m/s worth of propellant
- Fly the route builder to the _Midlands_ biome (the suggested location is a plateau or mesa west of _Greater Flats_)
- Complete that route (_Greater Flats_ to _Midlands_, should be 0 cost)
- Start a new route
- Fly back to the propellant dump on the _Greater Flats_
- Reload with propellant
- Complete the 0-cost route
- Return the route builder to **Minmus Shipyard**

### 01 Midlands Exotic Minerals

This first depot expansion is trivial. This is only one harvester, and the just-established Depot has exactly the power required to run this single module.

- Build **01 Midlands Exotic Minerals**
- Rendezvous **Skycrane** with **01 Midlands Exotic Minerals**
- Dock **01 Midlands Exotic Minerals** with **Skycrane**
- Land **Skycrane** in _Midlands_ biome
- Undock **01 Midlands Exotic Minerals**
- Connect **01 Midlands Exotic Minerals** to the Midlands biome depot
- Route the 10 Exotic Minerals production from Midlands to Greater Flats

### 02 Greater Flats Synthetics

Route these resources to Minmus Greater Flats

- 1 Food
- 1 Oxygen
- 5 Water
- 3 Material Kits

Build **02 Greater Flats Specialized Parts** at **Minmus Shipyard**. Fuel it and leave it in a parking orbit (eg: 15km).

Launch a **3.75m Crew Pod SSTO** carrying a **Crew Pod** with the following crew:

- Engineer
- Kolonist
- Mechanic
- Medic
- Miner
- Scientist
- Technician

Now get that crew to the **02 Greater Flats Specialized Parts** vessel:

- Rendezvous **Crew Transport** with **3.75m Crew Pod SSTO**
- Move the crew pod over to dock with **Crew Transport**
- Transfer the Supplies and Fertilizer resources from **3.75m Crew Pod SSTO** to the **Crew Transport**
- Send **Crew Transport** to Minmus
- Return the **3.75m Crew Pod SSTO** to **KSC** (or just deorbit it, or bring it to **Kerbin Shipyard** and disassemble it for parts)
- At Minmus, rendezvous **Crew Transport** with **02 Greater Flats Specialized Parts**
- Detach the **Crew Transfer Pod**
- Dock the **Crew Transfer Pod** with the lander

That is how we'll be transferring crew from **Kerbin** to **Minmus** for the rest of the **Minmus** campaign. For the **Mun** campaign we'll explore _WOLF Passenger Routes_, but one step at a time.

Now that **02 Greater Flats Specialized Parts** has crew:

- Land **02 Greater Flats Specialized Parts** at _Greater Flats_
- Connect the lander to the depot
- Transfer 5 Specialized Parts, 2 Alloys, 1 Synthetics from _Greater Flats_ to _Minmus Orbit_
- Transfer 1 Alloys from _Minmus Orbit_ to _Kerbin Orbit_
- Build an **A/E/R/S Hopper** shipyard component and dock it to **Minmus Shipyard**
- Connect the Alloys, Synthetics and Specialized Parts hoppers of **Minmus Shipyard** to the depot and start them

### 03 Midlands Agricultural Support

With Specialized Parts and Sythetics being manufactured there's a bit less pressure on resource reserves at **Minmus Shipyard**.

From here we're going to work towards producing Electronics and Robotics. To do that we will need to produce material kits to support the Electronics and Robotics production as well as to support maintenance of the depots. There will also be demand for food, water and oxygen.

The immediate next step is to get production of a surplus 5 food, water, oxygen and material kits at Greater Flats, allowing Greater Flats to no longer be dependent on imports of life support from orbit. To produce food at _Greater Flats_ we need to source _Fertilizer_ which means finding _Gypsum_.

After that life support capacity improvement, we'll pursue small increments in Alloys, Synthetics and Material Kits production followed by small increments in Robotics and Electronics production. The main constraint here is going to be limited supplies of those resources at **Minmus Shipyard** -- but this expansion project will be sipping from a very large barrel.

That's the basic road map, now let's get to work!

In the WOLF Tutorial save game, _Midlands_ have 20 abundance of _Gypsum_, 50 abundance of _Hydrates_ but no _Water_ (but we can extract _Water_ from _Hydrates_). The _Poles_  have 50 _Gypsum_ but no _Water_ or _Hydrates_. So for this _Fertilizer_ factory we'll expand the Midlands biome depot.

This depot lander requires the following to be transferred from Greater Flats:

- 1 Food
- 1 Oxygen
- 3 Material Kits

Send this crew:

- Engineer
- Kolonist
- Mechanic
- Medic
- Scientist

The process I've used for transferring crew is described in **02 Greater Flats Synthetics**. Launch the crew in a crew pod, dock the crew pod with the **Crew Transport**, rendezvous that craft with the lander, transfer the crew pod to the lander.

### 04 Greater Flats Food and Electronics

This one's pretty straight-forward: just use the water and dirt available in the Greater Flats along with the _Fertilizer_ we just started producing in the Midlands to produce lots of food. This lander will add 60 abundance of _Food_ to _Greater Flats_ which will be sufficient to supply the remaining Minmus depots.

To produce 1 abundance of _Electronics_ we need 5 _Material Kits_ and 5 _Synthetics_.

Arrange for 8 more _Exotic Minerals_ to be transferred to _Greater Flats_ from _Midlands_ if you haven't already taken care of that mountain of exports ready to be transferred.

Send this crew:

- Farmer
- Miner
- Technician

### 05 Greater Flats Robotics

No extra resources required for this one, just the crew:

- Miner
- Scientist
- Technician

Remember to keep deploying Depot Boxes to the remaining biomes on Minmus while waiting for all these crew to arrive.

### 06 Lowlands Polymers

With the four advanced materials taken care of, Minmus is now effectively self-sufficient. Take some time to deploy the remaining Depot modules to the remaining flats, Lowlands, Highlands, and Poles. As you deploy the depot modules, repeat the route-building process described in **Minmus Route Preparation** to establish routes from _Greater Flats_ to the new biome and back to _Greater Flats_. Remember to survey the WOLF Biome using the survey scanner nestled in the nose of the **Skycrane**.

Eventually we'll finish expanding Minmus just to have resources to produce _Prototypes_, _Colony Supplies_ and _Machinery_ anyway. _Colony Supplies_ in particular are important since they are required as part of the WOLF passenger transport system which we'll use to get crew to **Mun**. While flying rockets is fun, being a bus service can get tedious.

The immediate goal of this expansion is to produce the resources needed to provide **Mun Shipyard** with 15 _Material Kits_, 5 _Specialized Parts_, and 1 each of _Alloys_, _Electronics_, _Robotics_ and _Synthetics_.
_Polymers_ are needed for _Material Kits_ and _Synthetics_. More polymers is good!

Prepare for this depot expansion by transferring these resources to the **Lowlands** biome:

- 2 Fertilizer
- 1 Food
- 3 Material Kits

You'll need these crew for the depot expansion itself:

- Engineer
- Kolonist
- Farmer
- Mechanic
- Medic
- Miner
- Scientist
- Technician

Route the Exotics, Polymers and Synthetics produced by this expansion back to _Greater Flats_.

### 07 Flats Stage 1

This depot will be producing a small quantity of _Material Kits_, a lot of water, and laying the infrastructure for a second expansion to produce some more _Material Kits_ as more _Polymers_ become available.

- 1 Food

Crew:

- Engineer
- Kolonist
- Mechanic
- Medic
- Miner
- Scientist
- 2 x Technician

### 08 Highlands Material Kits

If you haven't already, establish the depot using a **Skycrane Depot Box** dropped off by the **Skycrane**. Make sure you survey the biome before taking off! Then establish a route from _Greater Flats_ to _Highlands_ and back to _Greater Flats_ using the procedure described in **Minmus Route Preparation**.

Imports:

- 1 Food

Crew:

- Engineer
- Kolonist
- Mechanic
- Medic
- Miner
- Scientist
- 2 x Technician

This gives us 7 extra _Material Kits_

### 09 Greater Flats Material Kits

Imports:

- 6 x Polymers (should already be provided by **06 Lowlands Polymers**)

Crew:

- Engineer
- Kolonist
- Miner
- 2 x Technician

This gives us 36 extra _Material Kits_. Between this and the Highlands depot previously deployed, that's a fine pile of _Material Kits_ to be sitting on. A lot of these will be consumed as _Colony Supplies_ which are required for WOLF passenger routes. More about that soon.

This lander requires 237,310 _Material Kits_. If you've followed the walkthrough your **Minmus Shipyard** will be producing 15,000 _Material Kits_ per day. Set an alarm (I use Kerbal Alarm Clock in preference to the built-in alarm clock) for the point in time that there will be enough _Material Kits_ to build this lander. Don't waste time with storage full of _Material Kits_!

### 10 Poles Exotic Minerals

The Poles doesn't have much that will help keep it self-sufficient so import the resources needed, and only build what's required to extract all those _Exotic Minerals_.

Transfer these supplies in:

- 1 Food
- 3 Material Kits
- 1 Oxygen
- 5 Water

The lander will need this crew:

- Engineer
- Kolonist
- Mechanic

Once that depot is established, transfer the _Exotic Minerals_ back to _Greater Flats_.

45,580 _Material Kits_.

### 11 Midlands Exotics and Food

We revisit Midlands to extract the remnant _Exotic Minerals_ and produce some food while we're at it.

Imports:

- 3 Material Kits

Crew:

- Farmer

200,887 _Material Kits_

### 12 Great Flats Specialized Parts

This one uses a heap of imported materials to produce _Specialized Parts_ in situ. It's a toss-up between importing _Exotic Minerals_ versus exporting lots of _Silicon_ and _Rare Metals_.

- 12 Exotic Minerals
- 1 Food
- 3 Material Kits
- 1 Oxygen
- 5 Water

The crew is

- Engineer
- Kolonist
- Mechanic
- Medic
- 2 x Miner
- Scientist
- 2 x Technician

155,580 _Material Kits_.

Exports:

- 25 x Specialized Parts

### 13 Flats Chemicals and Silicon

Crew:

- 2 x Miner
- Technician

155,530 _Material Kits_

Exports:

- 18 x _Chemicals_
- 12 x _Silicon_

### 14 Great Flats Rare Metals

Imports:

- 1 Food
- 4 Material Kits
- 1 Oxygen
- 5 Water

Crew:

- Miner
- Technician

130,530 _Material Kits_

Exports:

- 5 Food
- 18 Metals
- 70 Rare Metals

### 15 Highlands Rare Metals

Just one extractor using excess power.

Exports:

- 10 Rare Metals

9,230 _Material Kits_

### 16 Greater Flats Industry Park (teal)

This depot expansion will produce enough advanced resources (Sp/A/E/R/S) to get the Mun base up and running. There will be leftover Specialized Parts to send back to Kerbin for Colony Supplies.

Crew:

- Scientist
- Technician

Exports:

- 1 Alloys
- 1 Electronics
- 1 Robotics
- 1 Synthetics
- 25 Material Kits
- 35 Specialized Parts

70,530 _Material Kits_

### 17 Great Flats Fuel (violet)

Produce a bunch of fuel. This will contribute to resources for Mun Shipyard establishment.

Imports:

- 1 Material Kits

Crew:

- 3 x Geologist

Use these resources in Minmus Orbit, cancel the various transfers from Kerbin Orbit to Minmus Orbit. Send the excess fuel from Kerbin Orbit to Mun Orbit Then connect Mun Shipyard's fuel hoppers and start them up.

187,280 _Material Kits_

### 18 Flats Fuel (orange)

Produce more fuel. This will contribute to resources for future expansion shipyards.

Imports:

- 1 Material Kits

Crew:

- 3 x Geologist

As before, uses these resources to displace Minmus Orbit imports, then export to Kerbin Orbit, and then Mun Orbit.

187,280 _Material Kits_

### 19 Highlands Life Support

Produce water and oxygen for life support systems.

Export to Kerbin Orbit and from there to expansion depots.

### 20 Midlands Metals (teal)

Crew:

- 2 x Miner
- 2 x Technician

### 21 Lesser Flats Silicon (violet)

On the last stretch, just gathering up the remaining resources that will contribute to Specialized Parts production.

Imports:

- Food
- 3 x Material Kit
- Oxygen
- 5 x Water

Crew:

- Engineer
- Kolonist
- Mechanic
- 3 x Miner
- 3 x Technician

Exports:

- 36 x Silicon

### 22 Greater Flats Specialized Parts (orange)

Our final installation for Minmus. What a journey it's been! Here we just produce some more _Specialized Parts_ which will be almost immediately swallowed up by the next WOLF feature the Walkthrough will be exploring which is _passenger routes_.

Crew:

- 2 x Miner
- 4 x Technician

Exports:

- 80 x Specialized Parts

### Build Routes Back to Kerbin Orbit

With that deployment done there is a cornucopia of _Specialized Parts_ abundance to transfer to _Kerbin Orbit_. Build another route from _Greater Flats_ to _Minmus Orbit_, then from _Minmus Orbit_ to _Kerbin Orbit_ using the technique that has worked so well so far:

1. Remove what propellant you can
2. Start the route
3. Load up with propellant
4. At the other end you should have a zero cost route

This new route should be enough to carry about 80 _Specialized Parts_ back to Kerbin. There's still a quantity remaining, you could send the route builder back to Minmus to expand that route, since the **Kerbin Shipyard** is going to need time to produce the fuel required to get the Mun fleet provisioned.

## Passenger Transport

Some time back you built a **KSC Passenger Terminal**. Find it and move it next to the launch pad. Make sure the _WOLF Terminal_ module is connected to the depot.

### Passengers from KSC to Kerbin Orbit

Creating passenger routes is done similarly to creating cargo routes, but there are extra requirements at the origin depot:

- 2 Colony Supplies per luxury berth (colony supplies require specialized parts)
- 2 habitation per luxury berth
- 2 life support per luxury berth
- passenger route must start within 500m of a _WOLF Passenger Terminal_
- passenger route must finish within 500m of a _WOLF Passenger Terminal_

For this part of the walkthrough we'll want to set up a 15 luxury passenger route (luxury routes are faster, but consume double the resources per seat of economy routes). This will require 30 _Habitation_, 30 _Life Support_, and 30 _Colony Supplies_. The catch is that the _WOLF Fabricator Module_ will produce batches of 5 _Colony Supplies_ with these inputs:

- 5 x _Colony Supplies_ (Fabricator)
  - 5 x _Machinery_ (Fabricator)
    - 3 x _Material Kits_
    - 2 x _Specialized Parts_
  - 3 x _Material Kits_
  - 2 x _Specialized Parts_

Thus with 1 _WOLF Fabricator Module_ configured for _Colony Supplies_ paired with another configured for _Machinery_, we can produce 5 x _Colony Supplies_ for a total of 6 x _Material Kits_ and 4 x _Specialized Parts_.

Assemble six of those pairs (6 fabricators producing _Colony Supplies_, 6 fabricators producing _Machinery_) and add two _WOLF Habitation Module_ and one _WOLF Life Support Module_ to produce:

- 30 x _Colony Supplies_
- 40 x _Habitation_
- 30 x _Life Support_

This will consume:

- 36 x _Material Kits_
- 24 x _Specialized Parts_

There are other considerations along the way such as life support and crew (remembering that crew dedicated to the WOLF depot consume habitation and life support themselves), maintenance and power. I've packaged this up as **02 Orbit Colony Supplies** in the VAB under **WOLF Depot Landers/Kerbin**.

The _Specialized Parts_ will be coming from Minmus, so let's sort out the 36 _Material Kits)_ required for this expansion.

### 03 Grasslands Material Kits

This is the first of two depot expansions to produce the _Material Kits_ required for production of the _Colony Supplies_ required for the passenger route from _KSC_ to _Kerbin Orbit_. Note that the prebuilt assembly is the **RBR Trailer** with solar power and a Malemute cabin. We don't need to expand route capacity for this installation so no giant Route Builder Rover here.

Deploying this expansion can be done similarly to previous Kerbin ground deployments:

1. engage the brakes
2. open Bon Voyage Control Panel from the Malemute Cab PAW
3. select "Use Batteries"
4. set the destination coordinates
5. GO!
6. Switch to a different scene and wait

Being solar powered, this depot deployer will run on batteries until that energy is used up, then halt until the sunshine is available.

Crew:

- 2 x Miner
- 3 x Technician

Exports:

- 19 _Material Kits_

### 04 Grasslands Material Kits

This is the second of two depot expansions to produce the _Material Kits_ required for the _KSC_ to _Kerbin Orbit_ passenger route.

Deploying this one is basically a repeat of **03 Grasslands Material Kits**.

Note to self: be patient and don't try sending two rovers to the same coordinates otherwise they will spawn inside each other and explode.

Crew:

- Engineer
- Kolonist
- 3 x Miner
- 3 x Technician

Exports:

- 24 _Material Kits_

### 05 KSC Colony Supplies

Import those 24 x _Specialized Parts_ to _KSC_ from **Minmus** via _Kerbin Orbit_ and deploy **05 KSC Colony Supplies** from the SPH.

Crew:

- Technician

### Establish KSC to Orbit Passenger Route

And now we get to what all that effort was about: creating a passenger route from KSC to Kerbin Orbit. Prepare **5m 15 Passenger SSTO** for launch:

- Transfer propellant to KSC Passenger Terminal
- Start the passenger route by selecting _Connect to origin depot_ under the _WOLF Crew Transporter_ heading
- Transfer propellant back to the route builder
- Launch to orbit
- Rendezvous with **Kerbin Shipyard**
- Finish the passenger route by selecting _Connect to destination depot_ under the _WOLF Crew Transporter_ heading
- Dispost of **5m 15 Passenger SSTO** as you see fit

**Note: If you get a warning that you must be within 500m of a terminal in the same biome** this will be because you haven't connected the **KSC Passenger Terminal** to the depot yet. Do that, then you'll need to change scenes and come back to the launch so that the WOLF modules will know that there's a depot in that biome now.

### Passenger Transfers

The next infrastructure you're going to deploy is **07 Orbit Colony Supplies**. It requires 5 crew (see the crew list i nthe following section). Up till now we've launched crews from KSC in crew pods. Now there's a passenger route from KSC to Kerbin Orbit, so let's use that.

Put these crew into something that holds crew (eg: the **07 Orbit Colony Supplies** craft itself, which will let you check the _Planner_ before launching to make sure everything's set up correctly) and "launch" the crew holder from the VAB.

![KSC Launchpad with 02 Orbit Colony Supplies on pad and KSC Passenger Terminal in background][KSCORBSUPPPAD]

Open the _Crew Transfers_ interface using the icon that looks like a plane taking off.

![Crew Transfers Interface showing one flight available from Kerbin KSC to Kerbin Orbit][CREWTRANSUI]

On the left you have a list of flights that are available. The icons next to the flights will be a plane taking off to indicate an available departing flight, a plane landing to indicate a crew transfer that has completed (more on that later) or a flying rocket to indicate a crew transfer flight that is in progress.

For the moment there is only one flight, which is the one we just established from _Kerbin KSC_ to _Kerbin Orbit_. Select that flight and the middle column will be populated with the flight details and available crew.

The flight details pane show where this flight is leaving from and where it travels to, how many economy or luxury seats are available, and how long the flight will take (in this case "1d 0h 0m").

On the right is the departure pane. Once you add crew to the flight you can click "Launch!" to commit those crew to the flight. At this point, select all the crew in the middle pane and click "Launch!"

The right hand pane of the Crew Transfers window should now show only the delay until the flight arrives:

![Crew Transfers Interface showing the KSC to Orbit flight is in progress and will arrive in about 1d][CREWTRANSINFLGHT]

Now recover the craft that previously held the crew.

When the flight has reached Kerbin Orbit, head to the **Kerbin Shipyard** and open the _Crew Transfers_ window through the _Show Terminal Window_ action in the _WOLF Terminal_'s PAW, then:

1. Select the flight that has arrived at this terminal from the left pane (the icon of a plane landing, standard "arrivals" ideogram)
2. Select all the crew from the middle pane
3. Select the terminal that you want passengers to disembark at from the dropdown in the right-hand pane
4. Disembark

This is the scene in my game:

![Kerbin Shipyard with terminal PAW open and Crew Transfers Window showing arrived flight, selected crew and disembarking terminal][KSYCREWARRIVE]

### 06 Grasslands Material Kits

Produce some more _Material Kits_ to support the passenger route from _Kerbin Orbit_ to _Mun Orbit_. You'll need to expand the route for Grasslands back to KSC so this one is a trailer deployed by the Route Builder Rover. Remember to put a pilot in the RBR itself to get it moving faster when using Bon Voyage to move rovers. This rover is un-steerable due to using Rovemax Model XL3 wheels.

Crew (in the Karibou Crew Cabin, which you might need to re-attach in order to convince KSP that the crew seats exist):

- Technician

Exports:

- 60 x _Material Kits_ (send these to Kerbin Orbit)

### 07 Orbit Colony Supplies (SPH)

This Kerbin Orbit depot expansion simply adds the required _Colony Supplies_, habitation and life support to allow a passenger route builder to link **Kerbin Shipyard** to the imminent **Mun Shipyard**.

Once the crew that you transferred have arrived, build this craft and transfer the crew aboard:

1. undock the crew pod
2. dock the crew pod with **Kerbin Shipyard**
3. transfer the crew from the WOLF Terminal to the crew pod
4. undock the crew pod
5. dock the crew pod with **O7 Orbit Colony Supplies**
6. connect to depot.

Imports:

- 2 x Food
- 41 x Material Kits (from Kerbin)
- 2 x Oxygen
- 24 x Specialized Parts (from Minmus)
- 10 x Water

Crew:

- Engineer
- Kolonist
- Mechanic
- 2 x Technician

## The Mun Expansion

The Mun expansion will be a rehearsal for further expansion into the Kerbol system. The basics will be:

- send a seed fleet of shipyard, cargo route builder and passenger route builder
- if you are planning to use nuclear powered rovers, send the **Reactor Maintenance** vessel with an engineer (and when establishing the shipyard make sure to include **Passenger Quarters** along with the **Passenger Terminal** to get the Kerbal back to work)
- establish the orbital depot
- finish the cargo and passenger routes
- transfer WOLF resources using WOLF cargo routes
- establish communications network
- build a route builder rover (and land it)
- build the WOLF infrastructure at the shipyard
- import crew from Kerbin via the WOLF passenger routes

Before you go further, tie up your loose ends. Make sure all the resources you want from Minmus are transferred to Kerbin Orbit, all the resources you want from Kerbin are transferred to Kerbin Orbit, and you have the **Orbital Route Builder 75** and **5m 15 Passenger SSTO** parked in orbit around Kerbin.

At this point in the game there should have at least the following available in Kerbin Orbit:

- 1 Alloys
- 1 Electronics
- 1 Robotics
- 1 Sythetics
- 5 Specialized Parts
- 35 Material Kits

You can free up more resources by disconnecting the Minmus Shipyard hoppers from the depot, we aren't going to be using those resources again during the walkthrough.

Check that you have 30 spare of each of Colony Supplies, Habitation and Life Support to build the passenger route to the Mun.

With all those items checked, we can start on the Mun expansion!

### Mun Shipyard

This expansion to the Mun will serve as a template for expansions to other worlds. Here's the rough game plan for establishing the **Mun Shipyard**:

- Build **Expansion Shipyard** at **Kerbin Shipyard** and name it **Mun Shipyard**
- Provide **Mun Shipyard** with starter resources of _Alloys_, _Electronics_, _Robotics_ and _Prototypes_ (basically enough to build the A/E/R/S Hopper)
  - 100 Alloys
  - 150 Synthetics
  - 20 Robotics
  - (No electronics required to bootstrap)
  - (Material Kits and Specialized Parts will arrive via WOLF Transfers)
- Send **Mun Shipyard** to _the Mun_ along with the passenger and cargo route builders
- Once at _the Mun_ put **Mun Shipyard** into a circular 30km orbit at 0 inclination
- Establish cargo route from _Kerbin Orbit_ to _Mun Orbit_
- Transfer 15 _Material Kits_, 5 _Specialized Parts_, 1 _Alloys_, 1 _Electronics_, 1 _Robotics_ and 1 _Synthetics_ to _the Mun_
- Connect _Material Kits_ and _Specialized Parts_ hoppers to the depot
- Build the **A/E/R/S Hopper** shipyard component and connect it to the depot
- Build the **Passenger Terminal** shipyard component and connect it to the depot
- Build the **Manufacturing Hopper** shipyard component and connect it to the depot (provide an extra 20 _Material Kits_ to hook the hoppers up, you can borrow these from Minmus and Kerbin shipyards)

There are no step-by-step instructions but what you want to end up with here is the **Expansion Shipyard** at the Mun, with the A/E/R/S hopper component and passenger terminal component attached, all the hoppers connected and (with the next section) the CommNet expanded to provide coverage for vessels in orbit and rovers on the surface.

![The Author's example Mun Shipyard with Manufacturing Hopper, A/E/R/S Hopper and Passenger Terminal attached][MUNYARD]

### Mun CommNet

- Build **Satellite Bundle** and deploy the relay sats
  - Deployer should go to 377.355km x 621.4765km orbit (4h neat)
  - Release one relay satellite just before each periapsis
  - Circularise each relay satellite at periapsis (377.355km circular orbit, 3h neat)
  - Double-check the deployer's orbit between deployments
  - When three relays are deployed, put the deployer into a 200km polar orbit
  - Deploy the scanner and perform an orbital analysis

You can tune the orbital period to your liking using tools such as the [Resonant Orbit Calculator][RESORBCALC] we used back in the Minmus expansion. These numbers are only a recommendation. Just remember that a surface-synchronous orbit is not possible due to the Mun's SOI being smaller than the required orbit.

### Mun Passenger Routes

Now to build a passenger route from _Kerbin Orbit_ to _Mun Orbit_. Combined with the route from KSC to Kerbin Orbit, this will reduce the workload of launching crew pods, docking to crew transport, rendezvous at Mun Shipyard and transferring the crew pod back and forth.

To produce the passenger route from _Kerbin Orbit_ to _Mun Orbit_ you'll need to meet the requirements for starting a passenger route at **Kerbin Shipyard**. This means ensuring that _Kerbin Orbit_ has sufficient _Colony Supplies_, _Habitation_ and _Life Support_ to start the new route. Using the 15 luxury berth **5m 15 Passenger SSTO**, you'll need 30 of each of those resources. This should have been provided with the **07 Orbit Colony Supplies** expansion for Kerbin Orbit.

As with the previous route building exercise, start the route near a WOLF Terminal. In this case the terminal will be the **Kerbin Shipyard**:

1. Empty the route builder's propellant into the shipyard
2. Start the passenger route
3. Refuel the route builder
4. Transfer the route builder to the destination
5. Rendezvous with the destination terminal
6. Finish the passenger route

Note that you want to have the passenger terminal ready when the route builder arrives. The flight duration is based on how long it took your route builder to transit between the origin and destination stations. Thus to minimise transit time you might look at starting the route immediately  before initiating the transfer burn, and using a rocket with high delta-v to get the trip done quickly, and timing the arrival to ensure that the rendezvous with the destination station happens as soon as possible.

On the flip side, the rate of production of _Material Kits_ at the **Mun Shipyard** is about 15,000 a day and many of the depot landers we're going to build require hundreds of thousands of _Material Kits_, so the duration of the crew transfer flight doesn't really matter that much. Minimising the transfer time will be important for **Duna** however.

### Mun Depots

The aim here is the same as for **Minmus**: get the local shipyard to be self-sufficient, get some excess _Specialized Parts_ and _Material Kits_ production to support further expansion of the passenger network, then look at what else can be produced locally to contribute towards _Prototypes_ and _Colony Supplies_ production back at **Kerbin Shipyard**.

The critical path for **Mun** is getting the passenger terminal, route builder rover, and orbit to Farside Crater cargo route established.

Establish depots in the following biomes. The supplied locations are flat-ish and level-ish enough to land a rocket or park a rover, and the order will allow you to start setting up cargo routes and establishing the infrastructure while you establish the remaining depots ahead of landing the expansions:

- Canyons (18.150, -50.300) (18 9' 0"N, 50 18' 0"W)
- East Crater (-9.746, 84.452) (9 44' 45"S, 84 27' 7"E)
- East Farside Crater (7.109, -150.838) (7° 6' 32.4"N, 150° 50' 16.8"W)
- Farside Basin (28.514, -91.562) () (~1100m/s dv required to land)
- **Farside Crater** (-0.247, -58.873) (0 14' 48"N, 58 53' 2"W)
- Highland Craters (64.424, 173.655) (64 25' 41"N 173 40' 3"E)
- Highlands (0.372, -34.280) (0° 22' 19.2"N, 34° 16' 48"W)
- Lowlands (0.305, -0.530)
- Midland Craters
- Midlands (-0.97, 158.681)
- Northern Basin
- Northwest Crater (2.926, 17.980) (2 55'34"N 17 59'9"E)
- Polar Crater (50 52' 4"N 36 32' 59"W)
- Polar Lowlands (79.666, 108.266)
- Poles
- Southwest Crater (-28.202, 8.093) (28 9'55"S 8 14'53"E)
- Twin Craters (-5.916, 139.817) (5 54'56"S, 139 49' 1"E)

Canyons is unique in having Exotic Minerals and Rare Metals in one biome, from this one depot we can develop an abundance of 160 _Specialized Parts_ and 15 _Synthetics_ (ignoring allocaton of rare metals for alloys or polymers for material kits). Canyons can also be expanded to produce food, water and oxygen.

The highest abundance of manufactured items:

- 95 Material Kits from Twin Craters
- 125 Specialized Parts from Highlands

The highest sources of base materials are:

- 96 Chemicals from Canyons
- 130 Exotic Minerals from Polar Crater
- 68 Metals from East Farside Crater
- 52 Polymers from East Farside Crater
- 160 Rare Metals from Farside Basin
- 160 Silicon from Polar Crater

Life support:

- 140 Food, 78 water from Twin Craters
- 100 Food, 118 water from Highlands

### Mun Route Builder Rover

The **Route Builder Rover** has a nuclear power plant. To build it you need to get an Engineer to the **Mun Shipyard** with _Enriched Uranium_ in order to start the reactor. It will also help to get a pilot to the shipyard before landing the rover.

- Rendezvous the **Reactor Maintenance** craft with **Kerbin Shipyard** and transfer _supplies_
- Rendezvous the **Reactor Maintenance** craft with **Mun Shipyard** and dock
- Build the **Route Builder Rover**
- Transfer propellant from **Mun Shipyard** to **Route Builder Rover**
- Undock **Reactor Maintenance** from **Mun Shipyard**
- Dock **Reactor Maintenance** to **Route Builder Rover**
- Use the engineer in EVA to _Perform Maintenance_ on the **Route Builder Rover**'s nuclear reactor
- Undock **Reactor Maintenance** from **Mun Shipyard**
- Transfer **Reactor Maintenance** to a parking orbit

Land the **Route Builder Rover** at **Farside Crater**. Build routes from here to these biomes and back (in order, since this is where the depot landers will be going):

- Highlands
- East Farside Crater
- Twin Craters
- Canyons
- Farside Basin
- Polar Crater

Perform a survey at each biome as the RBR arrives there.

### Depot Deployment Checklist

Here's a handy checklist for managing these depot deployments with minimal fuss:

1. Depot is Established (land a Depot module and establish the depot)
2. Depot is Surveyed (RBR visit, scan using Surface Scanner)
3. Depot has cargo route to Farside Crater (RBR)
4. Depot has cargo route from Farside Crater (RBR)
5. Entire crew has arrived at Mun Shipyard
6. There are sufficient resources to build the lander

### 01 Farside Crater Material Kits

This first expansion sets up some basic infrastructure for food, water and oxygen production and happens to make some material kits on the side.

Crew:

- Engineer
- Farmer
- Kolonist
- Mechanic
- Medic
- Miner x 3
- Scientist
- Technician x 3

Materials:

- 417,436 x _Material Kits_
- 4,013 x _Specialized Parts_
- 1,044 x _Alloys_
- 3,578 x _Synthetics_
- 63 x _Robotics_

### 02 Highlands Specialized Parts

Imports:

- 4 x Material Kits

Crew:

- Engineer
- Farmer
- Kolonist
- Mechanic
- Medic
- Miner x 3
- Scientist
- Technician x 3

Exports:

- 30 x _Specialized Parts_

Materials:

- 463,596 x _Material Kits_
- 4,405 x _Specialized Parts_
- 3,935 x _Synthetics_

### 03 East Farside Polymers

Crew:

- Engineer
- Farmer
- Kolonist
- Mechanic
- Medic
- Miner x 3
- Scientist
- Technician x 3

Exports:

- 26 x _Polymers_

Materials:

- 438,596 x _Material Kits_

### 04 Twin Craters Polymers

Crew:

- Engineer
- Farmer
- Kolonist
- Mechanic
- Medic
- Miner x 3
- Scientist
- Technician x 3

Materials: 408,596 x _Material Kits_

### 05 Canyons Exotic Minerals

Imports:

- 2 fertilizer
- 4 material kits

Crew:

- Engineer
- Kolonist
- Farmer
- Mechanic
- Medic
- Miner x 2
- Scientist
- Technician x 2

Materials: 413,596 x _Material Kits_

### 06 Farside Basin Material Kits

Imports:

- 1 Food

Crew:

- Engineer
- Kolonist
- Mechanic
- Medic
- Miner x 2
- Scientist
- Technician x 3

Exports:

- 24 x _Material Kits_
- 160 x _Rare Metals_

Materials: 438,596 _Material Kits_

### 07 Canyons Electronics and Robotics

Imports:

- 11 x Material Kits
- 6 x Metals

Crew:

- 2 x Miner
- Scientist
- 2 x Technician

Exports:

- 1 x Alloys
- 1 x Electronics
- 1 x Robotics
- 1 x Synthetics
- 20 x Exotic Minerals
- 34 x Polymers

Build Cost: 183,395 Material Kits

### 08 Twin Craters Material Kits

Crew:

- 2 x Miner
- 4 x Technician

Exports:

- 80 x _Material Kits_

Build Cost: 371820

### 09 East Farside Crater Rare Metals

TODO: update to extract substrate (refine to polymers) as well

Prepare 110 route capacity between East Farside Crater and Farside Crater.

Imports:

- 1 x Material Kits

Crew:

- Kolonist
- 2 x Miner
- 2 x Technician

Exports:

- 60 x _Rare Metals_
- 30 x _Metals_
- 26 x _Polymers_

Build Cost: 320,615 Material Kits

### 10 Farside Crater Specialized Parts

Prepare a lot of _Material Kits_ and _Specialized Parts_ to contribute to _Colony Supplies_ for the **Duna** expansion.

Crew:

- Engineer
- Kolonist
- 3 x Miner
- 3 x Technician

Build Cost: 427,486 _Material Kits_

### 11 Highlands Specialized Parts

Imports:

- _Material Kits_ x 4

Crew:

- Engineer
- Kolonist
- 4 x Miner
- 6 x Technician

Exports:

- 95 x _Specialized Parts_

Build Cost: 448,596 _Material Kits_

### 12 Polar Crater Exotic Minerals

Imports:

- Food
- 3 x _Material Kits_
- 2 x _Refined Exotics_

Crew:

- Engineer
- Kolonist
- Mechanic
- Medic
- Miner
- Scientist
- 2 x Technician

Exports:

Hope you enjoy driving that rover... 205 materials to export here.

- 124 _Exotic Minerals_
- 1 _Rare Metals_
- 20 _Specialized Parts_
- 60 _Water_

Build Cost: 282,486 _Material Kits_

### 13 Farside Crater Colony Supplies

Now to use all those resources to build stuff. How about 100 Colony Supplies?

This will be sufficient to set up passenger routes to Duna (coming up in this walkthrough) and a couple of other places that you might want to explore on your own.

Crew:

- Miner
- Scientist
- 6 x Technician

Exports:

- 100 x _Colony Supplies_

Build Cost: 463,596 _Material Kits_

### 14 East Crater Exotic Minerals

This single-extractor depot expansion exploits the tiny amount of exotic mineral abundance in the East Crater biome.

Exports:

- 10 x _Exotic Minerals_

### 15 Farside Crater Water

Crew:

- Kolonist

Exports:

- 40 x Water

### 16 East Farside Polymers

Imports:

- 2 x Material Kits

Crew:

- Engineer
- 2 x Miner
- 2 x Technician

Exports:

- 24 x Polymers

### 17 Farside Crater Prototypes

Crew:

- 2 x Engineer
- Kolonist
- Mechanic
- 5 x Scientist

### Wrapping Up

Now you need to build a route from Farside Crater to Mun Orbit to Kerbin Orbit and transfer some Colony Supplies and Material Kits. For this stage of the Walkthrough you need 30 _Colony Supplies_ in Kerbin Orbit. The final tally for this chapter is to bring these resources to Kerbin Orbit and have them available for the **Duna Shipyard**:

- 15 Material Kits
- 5 Specialized Parts
- 1 Alloys
- 1 Electronics
- 1 Robotics
- 1 Synthetics

And for the 15 passenger route builder:

- 30 Colony Supplies
- 30 Habitation
- 30 Life Support

The life support and habitation should have been provided by the

## Duna Expansion

The Duna expansion is going to be done using WOLF systems where possible. This means using passenger routes to transfer crew, which means the first crew will arrive about 2 years after the shipyard is parked in orbit. Because the **Route Builder Rover** is nuclear powered, we need an engineer to service the nuclear reactor and a pilot to drive the rover -- to handle this I will send an engineer and a pilot in the **Reactor Maintenance** craft that serviced the **Mun Route Builder Rover**. Dock it with the **Crew Transport** and send that combined vessel with the two crew to Duna.

**NB**: you might find it useful to add the **Bulk Fuel Storage** module to the **Kerbin Shipyard**, or simply pay attention to refilling the various craft as propellant becomes available.

Sticking to the WOLF-only plan, build these ships and send them to Duna, try to get them to arrive in this order too:

- Duna Shipyard
- Cargo route builder
- Passenger route builder (remember to only start the passenger route immediately before the departure burn)
- Reactor Maintenance with Engineer and Pilot (if you plan to use the Route Builder Rover)

Remember to add the materials to the Duna Shipyard that it will need to build the **A/E/R/S Hopper**:

- 94 Alloys
- 145 Synthetics
- 20 Robotics

Before departure, double check that the WOLF abundance of the following is ready (as per _Wrapping Up_ in the Mun expansion writeup):

- 15 Material Kits
- 5 Specialized Parts
- 1 Alloys
- 1 Electronics
- 1 Robotics
- 1 Synthetics

Establish the shipyard at a "low" Duna Orbit (100km or less), then:

- connect the cargo route to the Duna:Orbit depot
- transfer 5 x _Material Kits_, 5 x _Specialized Parts_, and 1 each of Alloys, Electronics, Robotics and Synthetics from Kerbin:Orbit to Duna:Orbit
- connect the _Specialized Parts_ hopper and one _Material Kits_ hopper to the depot and start them up
- Deploy the Orbital Shipyard when you have 4000 _Material Kits_ (about 6 hours)
- If you have an engineer available, deconstruct the fuel tanks and engines that were used to deliver the **Duna Shipyard** to Duna (this will produce some _Material Kits_)
- Build the **A/E/R/S Hopper** and attach it to the shipyard (requires about 6 days of resource production)
- Build the **Passenger Terminal** and attach it to the shipyard (requires about 10 days of production)
- connect the passenger route to the Duna:Orbit depot
- set up relay satellites at 60 degrees and 120 degrees from Ike, in circular orbits with the same period
- build a **Skycrane** to establish depots using **Skycrane Depot Boxes**.
- deploy **Route Builder Rover** to link biomes with Cargo routes

From here the process is the same as the previous expansions:

1. 1 each A/E/R/S
2. Fuel to support depot landers
3. 15 Material Kits
4. 5 Fertilizer to support passenger terminal
5. 5 Specialized Parts

At this point Duna will be more or less self-sufficient apart from having to send crew from Kerbin.

### Relay Satellites

To provide communications coverage for all of Duna's surface, my preferred option is two satellites in synchronous orbit with Ike, then a triplet of relay satellites for Ike that will also provide coverage for the Ike-facing side of Duna.

Ike orbital period is 65 517.859s (3d 0h 11m 57.9s), and its orbit is slightly eccentric. A compatible circular orbit is 2,880km, though you don't need to be exact on altitude at long as you can get the orbital period correct.

My usual method for getting relay satellites into a decent spread is to use a resonant orbit. That doesn't work for Duna/Ike because Ike keeps getting in the way. What I do for Duna is simply build the two Relay 100 satellites and set them directly on a rendezvous with their assigned positions 120 degrees leading and lagging Ike.

Then launch a trio of small relay satellites for Ike. When you capture that satellite delivery to Ike's SOI, use the [Resonant Orbit Calculator][RESORBCALC] to figure out what orbital parameters the deployer will need to space the satellites out correctly. Note that you can't achieve surface-synchronous orbit at Ike because its SOI is too small. The important thing is to get all the satellites onto the same orbital period to within a few seconds. With that level of accuracy you should have decent coverage for years at a time.

### Establish Depots

With the relay satellites in place, use a Skycrane to establish the depots (remember to survey the biome before takeoff). Here are some relatively flat and level landing sites based on my previous exploration:

- Craters (0.425,114.490)
- Eastern Canyon (5.303,162.344)
- Highlands (-0.518,163.717)
- Lowlands (-0.030, 6.424)
- Midland Canyon (9.398, -2.374)
- **Midland Sea** (0.103,75.868) (0° 6' 10.8"N, 75° 52' 4.8"E) (build route to orbit from here)
- Midlands (-0.883,131.492) (0° 52' 58.8"S, 131° 29' 31.2"E)
- Northern Basin (10 30'32"N, 84 24'30"W) (10.577, -84.653)
- Northern Shelf (23.941,21.445)
- Western Canyon (0 7' 31"S, 59 12' 43"W)
- Polar Craters (-52.989,147.409) (52°59'20.4"S, 147°24'32.4")
- Polar Highlands (-55.011,136.542) (55° 0' 39.6"S,136° 32' 31.2"E)
- Poles (-45.469,151.586)

### 01 Midland Sea Material Kits

You should now have a passenger route set up between Kerbin Orbit and Duna Orbit. Time to put it to use. The Midland Sea biome is capable of producing most of the resources required to make Duna independent of Kerbin. The initial infrastructure will provide some _Material Kits_, then later expansions will add production for _A/E/R/S_, _Fuel_, _Fertilizer_ and _Food_. The next biome depot expansion for Duna will provide the extra resources that this depot requires (mostly _Metal_).

Imports:

- Food
- Oxygen
- 5 x Water

Crew:

- Engineer
- Kolonist
- Mechanic
- Miner
- 2 x Technician

The route building craft presented in the tutorial save has a Luxury capacity of 15 Kerbals, meaning that you can potentially send the crew for multiple depot landers depending on whether you're able to limit the crew per lander. This can be great for setting up the basic infrastructure to get A/E/R/S production up and running without having to wait several decades.

For this walkthrough, you should be able to get this crew and the crew for **02 Polar Craters Metals** into the same flight from Kerbin Orbit to Duna Orbit. Send the crews to Duna, and spend the transit time establishing depots and scanning resources. I found it helps to write down the names of the Kerbals that belong to each crew so that transferring kerbals from **Duna Shipyard** to the crew section of the depot landers is easier.

Remember you have time to explore the other biomes, and perhaps even send new shipyards and route builders to other worlds.

### 02 Polar Craters Metals

This depot will provide the metals, food, water and oxygen required by the Midland Sea depot.

When landing this craft with MechJeb 2 I found I needed to perform the initial plane change and de-orbit burn manually after which MJ2 was able to land at the destination fairly accurately even if it didn't land exactly where I wanted it.

Imports:

- 4 x Material Kits

Crew:

- Engineer
- Kolonist
- Farmer
- Mechanic
- Medic
- Miner
- Scientist
- Technician

Exports:

- 16 x Metals

### 03 Midland Sea A/E/R/S

Here's the final depot expansion for this walkthrough, where we upgrade _Midland Sea_ to provide **Duna Shipyard** with its final essential resources.

Crew:

- Medic
- 2 x Miner
- 2 x Scientist
- 2 x Technician

There are only 7 crew for this mission, feel free to design your own depot expansion for somewhere else (perhaps to build more Specialized Parts to ship back to Kerbin for Colony Supplies) and add the crew here. Remember to test-land each lander before you put crew in one! Quicksave is your friend.

Once this expansion is connected to the _Midland Sea_ depot, you can cancel the exports of A/E/R/S, 5 x Specialized Parts and 15 x Material Kits from _Kerbin Orbit_.

## WOLF Walkthrough Conclusion

This is the end of the walkthrough for now. In this walkthrough we've covered:

- The WOLF Dashboard
- The WOLF Depot Planner
- Using the planner to design a depot expansion
- Expanding infrastructure by delivering crew and equipment to a biome
- Establishing cargo and passenger routes
- Using cargo routes to provide startup resources for depots
- Using WOLF passenger routes to deliver kerbals between WOLF Passenger Terminals

You have the tools and training required to use the WOLF Industry system. Good luck with your adventures!

## Addendums

Herein lies all the cruft that didn't fit elsewhere.

### Route Builder Rover User Guide

Welcome to the Jameson Industries RBR-45, the ultimate electric rover for your USI WOLF industry needs!



[MRWOLFTS]: https://github.com/MaraRinn/WOLF-Tutorial-Ships "Mara Rinn's WOLF Tutorial Ships repository"
[RDWOLF1]: https://docs.google.com/document/d/1zft2Ka9gubOYQf4CQgvReTxpnP8_LQYNyHouEjQZqjw/edit "Roverdude's introduction to WOLF"
[RDCONV]: https://kerbal-forum-uploads.s3.us-west-2.amazonaws.com/monthly_2020_12/wolf.png.53d635bf5f1f4cc0e4e2f6286409d827.png "Roverdude's resource conversion diagram"
[RDTRAN1]: https://docs.google.com/document/d/1BEqW60RrnYiVJKpAIFHAUqhdBrzbwwQ7KsaJ8hZjH4w/edit "Roverdude's introduction to transport credits"
[USIRELEASES]: https://github.com/UmbraSpaceIndustries/UmbraSpaceIndustries/releases "Umbra Space Industries combined package releases"
[CRPRELEASES]: https://github.com/UmbraSpaceIndustries/CommunityResourcePack/releases "Community Resource Pack releases"
[KSPROOT]: https://wiki.kerbalspaceprogram.com/wiki/Root_directory "Where to find the KSP root directory"
[RESORBCALC]: https://meyerweb.com/eric/ksp/resonant-orbits/ "KSP Resonant Orbit Calculator"
[TransferWindows]: https://docs.google.com/spreadsheets/d/1TOTvHIGdhWzK3FJC-DPzM1dQjXYcS_Mlbfs6rFD0hnU/pub?single=true&gid=0&output=html "Transfer windows for the first five years"

[AddOnInstallation]: Screenshots/AddonInstallation.png "Drag the contents of the USI GameData folder to the KSP GameData folder, then drag the contents of the CRP GameData folder to the KSP GameData folder, overwriting the CommunityResourcePack folder that's already there"
[TutorialShipsInstall]: Screenshots/WOLFTutorialSaveInstall.png "Drag the WOLF Tutorial folder from the WOLF Tutorial package to the Kerba Space Program saves folder, replacing any existing save of the same name"
[WolfDepotDeployerParts]: Screenshots/WOLFDepotDeployerParts.png "Runway scene with WOLF Route Builder Rover showing WOLF related parts with PAWs open for Surface Scanner, WOLF Transport Computer and Bon Voyage controller"
[WolfDashboardHarvestableResourcesEmpty]: Screenshots/WolfDashboardHarvestableResourcesEmpty.png "Runway scene with WOLF Dashboard open to Harvestable Resources pane showing no biomes with harvestable resources because they have not been scanned"
[WolfDashboardHarvestableResourcesScannedBiome]: Screenshots/WolfDashboardHarvestableResourcesScannedBiome.png "SPH scene with WOLF Dashboard open to Harvestable Resources pane showing resource abundance for freshly scanned biome"
[SPHWOLFEMPTY]: Screenshots/SPHWOLFEMPTY.png "SPH scene with WOLF Dashboard open to Depots pane showing no depots"
[SPHsceneFabricatorModuleWOLFDashboardPlanner]: Screenshots/SPHsceneFabricatorModuleWOLFDashboardPlanner.png "SPH scene with WOLF Dashboard open to Planner pane and WOLF Fabricator Module as the first part of a new vessel"
[SPHSCENE2MATKITS]: Screenshots/SPHSCENE2MATKITS.png "SPH scene showing WOLF infrastructure required to support creation of 2 Material Kits abundance"
[WOLFDEPOTPAWESTABLISH]: Screenshots/WOLFDEPOTPAWESTABLISH.png "WOLF Depot Module with PAW showing Establish depot action"
[WOLFDASHKERBINDEPOTBONUS]: Screenshots/WOLFDASHKERBINDEPOTBONUS.png "WOLF Dashboard showing the new KSC Biome Depot with bonus resources awarded to Kerbin-based depots"
[RUNWAY01KSCMATKITSCONNECT]: Screenshots/RUNWAY01KSCMATKITSCONNECT.png "Runway scene with WOLF expansion. PAW open showing Connect to Depot action"
[RUNWAYWOLFDASHNEWKSCDEPOTPRODUCTION]: Screenshots/RUNWAYWOLFDASHNEWKSCDEPOTPRODUCTION.png "Runway scene with WOLF Dashboard showing new production added"
[RUNWAYDEPOTBONVOYAGE]: Screenshots/RUNWAYDEPOTBONVOYAGE.png "Runway scene with WOLF Depot Deployer Rover PAW and Bon Voyage control panel with destination set"
[KERBINSHORESDEPOTDEPLOYMENT]: Screenshots/KERBINSHORESDEPOTDEPLOYMENT.png "Kerbin Shores scene with WOLF Depot Deployer. The depot and trailer are decoupled and Surface Scanner PAW is open. There are numbers 1, 2 and 3 indicating the order of operations."
[KERBINSHORESDEPOTDASHBOARD]: Screenshots/KERBINSHORESDEPOTDASHBOARD.png "Kerbin Shores scene with WOLF Dashboard open to Depots pane showing new Kerbin Shores depot"
[SPHDDRMaterialKitsAndCrew]: Screenshots/SPHDepotDeployer5MaterialKitsTrailer.png
[ShoresDepotDeployerConnectOriginDepot]: Screenshots/ShoresDepotDeployerConnectOriginDepot.png "Mountains scene with WOLF Depot Deployer rover showing the Transport Computer PAW. The 'connect to origin depot' action is visible."
[KSCDepotDeployerCoonectDestinationDepot]: Screenshots/KSCDepotDeployerCoonectDestinationDepot.png "WOLF Depot Deployer rover at KSC with 'connect to destination depot' action visible in the Transport Computer PAW"
[SPHWOLFDASHSTARTERPRODUCTION]: Screenshots/SPHWOLFDASHSTARTERPRODUCTION.png "SPH scene with WOLF dashboard showing starter depots expanded with completed production of material kits, fuel, food, oxygen, water and fertilizer"
[SPHWOLFDASHROUTESPANE]: Screenshots/SPHWOLFDASHROUTESPANE.png "SPH scene with WOLF dashboard open to routes pane showing starter routes established during depot construction"
[SPHWOLFDASHMANAGETRANSFERS]: Screenshots/SPHWOLFDASHMANAGETRANSFERS.png "SPH scene with WOLF Dashboard showing the Manage Transfers interface"
[KSCTransferMaterialKitsGrasslandsToKSC]: Screenshots/KSCTransferMaterialKitsGrasslandsToKSC.png "KSC scene with Transfer Resources interface showing a new transfer of 6 MaterialKits from Grasslands to KSC"
[KSCTransfersFromHighlandsMountainsShores]: Screenshots/KSCTransfersFromHighlandsMountainsShores.png "KSC scene with WOLF Dashboard showing transfers from highlands, mountains and shores to KSC"
[SPHRouteBuilderRover]: Screenshots/SPHRouteBuilderRover.png "SPH scene showing Route Builder Rover"
[KSCRouteBuilderRoutesBuilt]: Screenshots/KSCRouteBuilderRoutesBuilt.png "KSC scene with WOLF Dashboard open to the Routes pane. There are a number of routes built between KSC and the various biomes, expanded with the 45 payload capacity Route Builder Rover"
[SmallSSTORocketStartRouteAtLaunch]: Screenshots/SmallSSTORocketStartRouteAtLaunch.png
[SmallSSTORocketRouteCost30]: Screenshots/SmallSSTORocketRouteCost30.png
[KERB375ROCKETCREDITS]: Screenshots/KERB375ROCKETCREDITS.png
[WOLFSSTO0CREDITS]: Screenshots/WOLFSSTO0CREDITS.png
[SSTORTCOST8]: Screenshots/WOLFSSTOinOrbitWithRouteCost8.png "The WOLF SSTO craft in orbit with Transport Computer PAW open showing route cost of 8"
[ES96RTCOST85]: Screenshots/ES96PythonInOrbitWithRouteCost85.png "The ES-96 Python in orbit with Transport Computer PAW open showing route cost of over 80"
[VABWOLFTutorial100TransportCredits]: Screenshots/VABWOLFTutorial100TransportCredits.png
