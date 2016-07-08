# StarCraftFourPoolAI

A basic artificial intelligence for Starcraft: Broodwar running a 4 Pool build.

<strong>How to Run</strong>
- Install Starcraft: Broodwar and update to version 1.16.1.
- Download the latest version of BroodWar API [here](https://github.com/bwapi/bwapi).

If building from source:
- Download this repo and place the files in the BWAPI directory.
- Build FourPool.sln in Microsoft Visual Studio.

The already compiled DLL is also available in this repository.

- Copy the DLL (FourPool.dll) to bwapi-data/AI/ in your Starcraft directory.
- Run ChaosLauncher (as admin) found inside your BWAPI directory.
- Tick "BWAPI Injector (1.16.1) RELEASE" and hit config.
- Change "ai = bwapi-data/AI/ExampleAIModule.dll" to "ai = bwapi-data/AI/FourPool.dll" and close the text file.
- Hit start in ChaosLauncher, this should run SC:BW.
- Start a single player custom game with Zerg as your race and the AI should start working immediately.
