Welcome to Drconfused madness!

	Drconfused Oil Exctractor
		Current version 0.04
			
			**based on Stallionsden mining machine**

				
Contents 
* 	WHATS IN THE MOD?
*	TO DO/WISH LIST
*	VERSION HISTORY
*	MADNESS NOTES
*	MODDERS NEED TO KNOW BASIS
*	ICON IMAGE USE


<!--	WHATS IN THE MOD?	-->
	Adds an Oil and Gas extractor.
		-Control Panel block that changes into a gas pump when its ready to be looted. Loot it and it changes back to the control panel
		-Loot possibilities in the Extractor =
			-Gascan
			-Oil Shale
			-Oil
			-Terrain Blocks:
				-Oil Deposit
				-Oil and Sand
				-asphalt
				-
			-Paraffin wax
			-Tar
		
			
		-New recipes:
			-candles using the paraffin wax
			-Torch using tar,cloth, wood
			-DuctTape using tar and cloth
			-Tar can be made from asphalt at the chemistry station
		
		-New fuel and recipe for Motor Tools (auger and chainsaw) that requires 80 gas cans and 2 oil to make 100 MotorToolFuel. **Currently does not register in the lower right for ammo count**
		

<!--	TO DO/WISH LIST	-->
	1. loot.xml
		Balance the timing and loot available
			-after testing the initial release was grossly low for its time commitment, without it giving a buff of some sort its likely to be a waste of time and space that could be focused on other things, especially during a zombie apocolypse.
			-the 2nd revamp of loot, increased the drop rates but still I find to low for the intended use for my play style.
			-after looking at the loot rates in the vanilla files I found that 
	
	2. make an mid game and end game version so there are choices for difficulty in construction.
	3. Get unique blocks that are more specific to this mod concept.
	4. Add power requirements to the current setup.
	5. Add in proper animation so it appears the machine is running.
	6. Make a refinery that is a workstation
		6.1 Equip within
				-barrel of gas
					
				-beaker
				-
			allows for oil to be converted to gas
			oil shale converted to gas or oil
			paraffin wax is able to be extracted
	7. MotorToolFuel to be counted as ammo in the lower right so that it can be monitored for amount.
	8. Make higher tier Extractors that have adjusted recipes but increase the loot found.
	9. A buff on closing the Mining Well that increases power tool usage, this gives incentive to return not just for oil.
	10. Questline base on Oil and Gas
	11. is there a method that makes it so the block has to be placed on a specific block? is so can I utlize that function to create something more profound for a oil and gas extractor?
		
	
<!--	VERSION HISTORY	-->
	0.04 	March 3rd 2019
		-increased loot value per loot cycle
			-I am much more happy with this round of loot, it may be to high but its closer to my play style than the previous releases.
		-removed Motor Tool Fuel as it doesn't seem to be working. Hopefully I address this issue.
	0.03	March 2nd 2019
		-increased values once again per loot cycle
		
	0.02	February 28th 2019
		-increased slightly the possible amount of loot per cycle.
		-added heatmap values to the oil extractor and OilShaleHere
		-active radius effect added so it acts like a campfire and warms the space around it
		-paraffin wax added as loot that is produced in the extractor 
		-candle recipe added to use paraffin wax in.
		-added MotorToolFuel as a fuel source for auger and chainsaw.
		-added Tar 
			-recipes for Duct Tape and Torch that use tar
			-asphalt can be turned into tar at the chem station
		

	0.01		February 26th
		Initial release
		
		
<!--	MADNESS NOTES	-->
	1. Can I require the block to need power? 
		1.1 if yes how do I set the power need for it?
		1.2 Instead of needing power I will require a battery and engine in the recipe
		
	2. What are the textures I want to use with the initial block?
		2.1 I notice Stallionsden used the code 
				[CODE]
				<property name="Texture" value="346,345,341,345,262,345"/>
				[/CODE]
			to put the oven textures on.
		2.2 I chose to use the control panel block because it just seemed to fit a little more with the mod idea.
		
	3. Can I make the upgraderate a random value?
		What are all the different random modifiers?
		will IsRandom work with UpgradeRated?
			<property name="UpgradeRated.IsRandom"/>
	4. Turn ammoGasCan into an 
			<property name="Class" value="ExchangeItem"/>
			When filling up any item with AmmoGasCan return item emptyJerryCan
			ExchangeItem emptyJerryCan at Chemstations/GasPumps/OilExtractors
	5. Add in heatmap values
				<property name="HeatMapStrength" value="1.5"/>
				<property name="HeatMapTime" value="1200"/>
				<property name="HeatMapFrequency" value="25"/>
				
	6. Add in sound values

	7. would SleeperSmellSenseThreshold be a factor in items like this too?
	
	8. Loot.xml
		1. how can I use the same id but have different variants of drops? from different containers that use the same id?
		
		2. looking through the vanilla lootcointainers to assess what count uses they define and look at the larger counts
			<!-- gas pump loot -->
				<lootcontainer id="64" count="30,500" size="8,4"
		
		3. Should I define a loot group for th Mining Well?
		
	9. buffs.xml
		possibilities in buffing through the lootcontainer. We find this note in the xml.txt by TFP
			Optional attributes of a lootcontainer:
				"buff"
				"buff_chance"
				
		buff idea 1
			increase oil and gas related items sell value 
			
		buff negative
			increased smell value for a time that can attract the zeds
			
		

<!--	MODDERS NEED TO KNOW BASIS  -->
	exportcurrentconfigs - 
		enter into the console in game and a file will compiled that contains all the config changes that are loaded and from what mod. It will tell you the path

<!-- 	ICON IMAGE USE	-->


-Drs_MotorToolFuel
	https://www.maxpixel.net/Canister-Fuel-Metal-Isolated-Gasoline-Canister-Old-2460103







