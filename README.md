# StarCraftFourPoolAI

A basic artificial intelligence for Starcraft: Broodwar running a 4 Pool build. Made possible by Adam Heinermann's [Broodwar API](https://github.com/bwapi/bwapi).

<strong>How to Run</strong>
- Install Starcraft: Broodwar and update to version 1.16.1.
- Download the latest version of Broodwar API [here](https://github.com/bwapi/bwapi).

If building from source:
- Download this repo and place the files in the BWAPI directory.
- Build FourPool.sln in Microsoft Visual Studio.

The already compiled DLL is also available in this repository in Release/FourPool.dll.

- Copy the DLL (FourPool.dll) to bwapi-data/AI/ in your Starcraft directory.
- Run ChaosLauncher (as admin) found inside your BWAPI directory.
- Tick "BWAPI Injector (1.16.1) RELEASE" and hit config.
- Change "ai = bwapi-data/AI/ExampleAIModule.dll" to "ai = bwapi-data/AI/FourPool.dll" and close the text file.

To run only the AI:
- Hit start in ChaosLauncher, this should run SC:BW.
- Start a single player custom game with Zerg as your race and the AI should start working immediately.

To play against the AI:
- Close ChaosLauncher and open ChaosLauncher - MultiInstance (as admin) instead.
- Make sure "BWAPI Injector (1.16.1) RELEASE" is ticked and configured as above, and also tick "W-MODE 1.02"
- Hit start to create the instance of SC that the AI will play.
- Go back to ChaosLauncher - MultiInstance and untick "BWAPI Injector (1.16.1) RELEASE" and hit start to create the instance of SC that you will play (you can untick "W-MODE 1.02" if you want to play fullscreen).
- Create a Multiplayer > Local PC game, make sure both instances have joined the game.
- Set the AI's race to Zerg, start the game and the AI should start working immediately.
