# DevourClient

I wasn't home for 2 days so i made that, i learnt a lot about C# programming and about Unity IL2CPP game hacking.
DevourClient is a rather uncommon cheat for Devour, i've seen multiple cheats for this game but they all had some boring features such as ESP and stuff.
This cheat hasn't many features and some of them may broke with the time, but hey, spaming the chat with "Deez Nutz" is funny.
Also don't mind french comments lol, google translate is your friend !

ps : my computer was really bad so i couldn't do a lot of testing in game because it required too much time to load

## Detection rate

Well at this point i don't really know, i think there is some sort of native Unity anti cheat template but it doesn't seem active. You're fine, no anti cheat !

## Features
* An IMGUI menu thanks to UnityEngine
* Fully compatible with the new IL2CPP version of the game
* Detects if you're in game (with bad code lol), so no chances of crashing on main menu by activating features
* Detects the map you are playing on (useful for the instant win)
* Big Flashlight (allows your flashlight to light a lot more)
* Flashlight color customization (with a home made color picker)
* A chat spammer for Lobby and InGame chat (i couldn't do a text entry because of the limitations of [Il2CppAssemblyUnhollower](https://github.com/knah/Il2CppAssemblyUnhollower))
* Achievements unlocker (couldn't do all of them, my code is crashing for some reasons at some point, i may fix it, for now it's commented out)
* Doors unlocker (should work fine, though it doesn't seem to work sometimes)
* Keys teleporter (broken, works sometimes but doesn't TP all the keys for some reasons)
* LV 70 (puts you to the max level of the game !)
* Instant Win (allows you to win instantaniously on any map, works in singleplayer, but not as a client. May be working as host)

## Installation

0. Download the [release version](https://github.com/ALittlePatate/DevourClient/releases/) or [build it from source](https://github.com/ALittlePatate/DevourClient#building-from-source).
1. Install [MelonLoader](https://github.com/LavaGang/MelonLoader/releases/tag/v0.4.3) to Devour.
2. Start your game. A cmd should appear, don't close it, MelonLoader is installing and decompiling Devour's game assemblies.
3. Wait for the process to finish, once it's done close the game.
4. Put the DevourClient.dll file inside `C:\Program Files (x86)\Steam\steamapps\common\Devour\Mods` folder.
5. Start the game, now you have successfully installed DevourClient. Use INSERT to open the menu

## Uninstallation

0. Delete the folders `MelonLoader`, `Mods`, `Plugins`, `UserData`, and the file `version.dll` from `C:\Program Files (x86)\Steam\steamapps\common\Devour`

## Building from source

0. Clone the repository
1. Install MelonLoader (see [Installation](https://github.com/ALittlePatate/DevourClient#installation))
2. Open the solution file in Visual Studio (i used 2019, i don't know about the compatibility with the other versions)
3. Go to : Project --> Add a reference --> Browse --> Click on the browse button in the down right corner of the window.
4. Add those files :
* `C:\Program Files (x86)\Steam\steamapps\common\Devour\MelonLoader\MelonLoader.dll`
* `C:\Program Files (x86)\Steam\steamapps\common\Devour\MelonLoader\Managed\UnityEngine.IMGUIModule.dll`
* `C:\Program Files (x86)\Steam\steamapps\common\Devour\MelonLoader\Managed\UnityEngine.InputLegacyModule.dll`
* `C:\Program Files (x86)\Steam\steamapps\common\Devour\MelonLoader\Managed\bolt.user.dll`
* `C:\Program Files (x86)\Steam\steamapps\common\Devour\MelonLoader\Managed\bolt.dll`
* `C:\Program Files (x86)\Steam\steamapps\common\Devour\MelonLoader\Managed\UnityEngine.HotReloadModule.dll`
* `C:\Program Files (x86)\Steam\steamapps\common\Devour\MelonLoader\Managed\UnityEngine.UI.dll`
* `C:\Program Files (x86)\Steam\steamapps\common\Devour\MelonLoader\Managed\UnityEngine.CoreModule.dll`
* `C:\Program Files (x86)\Steam\steamapps\common\Devour\MelonLoader\Managed\Il2Cppmscorlib.dll`
* `C:\Program Files (x86)\Steam\steamapps\common\Devour\MelonLoader\Managed\Assembly-CSharp.dll`
* `C:\Program Files (x86)\Steam\steamapps\common\Devour\MelonLoader\Managed\UnityENgine.InputModule.dll`
* `C:\Program Files (x86)\Steam\steamapps\common\Devour\MelonLoader\Dependencies\Il2CppAssemblyGenerator\Il2CppUnhollower\UnhollowerBaseLib.dll`
* `C:\Program Files (x86)\Steam\steamapps\common\Devour\MelonLoader\Dependencies\Il2CppAssemblyGenerator\Il2CppUnhollower\UnhollowerRuntimeLib.dll`
5. Build the solutions in Release | Any CPU mode

## Contact

You can add me on discord at patate#1252

## Code used

For teaching me the basics :
* [A Begginner's Guide To Hacking Unity Games](https://www.unknowncheats.me/wiki/A_Beginner%27s_Guide_To_Hacking_Unity_Games)

For teaching me about the MelonLoader mods API and Il2Cpp specifications :
* [MelonLoader's quickstart documentation](https://melonwiki.xyz/#/modders/quickstart)
* [MelonLoader's Il2Cpp differences chapter in the documentation](https://melonwiki.xyz/#/modders/il2cppdifferences)

For teaching me about the UnityEngine API :
* [Unity User Manual 2020.3 (LTS)](https://docs.unity3d.com/Manual/index.html)

For decompiling and looking in the source code of the game :
* [dnSpy : a .NET debugger and assembly editor](https://github.com/dnSpy/dnSpy)

For teaching me the basics about Devour game hacking, and i pasted the Key TP hack and the non working part of the Achievements Unlocker from it :
* [DevourCheatMonoInjector](https://github.com/Glatrix/DevourCheatMonoInjector)

## Contributing

Open an [issue](https://github.com/ALittlePatate/DevourClient/issues/new) or make a [pull request](https://github.com/ALittlePatate/DevourClient/pulls), i'll be glad to improve my project with you !

## License

[GPL 3.0](https://www.gnu.org/licenses/gpl-3.0.md)
