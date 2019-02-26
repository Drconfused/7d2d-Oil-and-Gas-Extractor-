Welcome to Drconfused madness!

	Drconfused Oil Exctractor
		Current version 0.01
			
			**based on Stallionsden mining machine**

				
Contents 
* 	WHATS IN THE MOD?
*	TO DO/WISH LIST
*	VERSION HISTORY
*	MADNESS NOTES
*	MODDERS NEED TO KNOW BASIS


<!--	WHATS IN THE MOD?	-->
	Adds an Oil and Gas extractor.
		-Control Panel block that changes into a gas pump when its ready to be looted. Loot it and it changes back to the control panel
		-Loot possibilities in the Extractor =
			-Gascan
			-Oil Shale
			-Oil
			-Oil Deposit terrain block
			-Oil and Sand terrain block 


<!--	TO DO/WISH LIST	-->
	1. Balance the timing and loot available
	2. make an mid game and end game version so there are choices for difficulty in construction.
	3. Get unique blocks that are more specific to this mod concept.
	4. Add power requirements to the current setup.
	5. Add in proper animation so it appears the machine is running.
	
<!--	VERSION HISTORY	-->

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
	3. Can I make the upgraderate a random value?
		What are all the different random modifiers?
		will IsRandom work with UpgradeRated?
			<property name="UpgradeRated.IsRandom"/>
	4. Turn ammoGasCan into an 
			<property name="Class" value="ExhangeItem"/>
			When filling up any item with AmmoGasCan return item emptyJerryCan
			ExchangeItem emptyJerryCan at Chemstations/GasPumps/OilExtractors
	5. Add in heatmap values
				<property name="HeatMapStrength" value="1.5"/>
				<property name="HeatMapTime" value="1200"/>
				<property name="HeatMapFrequency" value="25"/>
				
	6. Add in sound values

	7. would SleeperSmellSenseThreshold be a factor in items like this too?


<!--	MODDERS NEED TO KNOW BASIS  -->
	exportcurrentconfigs - 
		enter into the console in game and a file will compiled that contains all the config changes that are loaded and from what mod. It will tell you the path









