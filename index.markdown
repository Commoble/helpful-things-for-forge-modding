---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

# layout: home
---
# Helpful Things for Making Mods with Forge for Minecraft 1.15

## Getting Started

```
0) Download and install the JDK for Java 8 and put it in your environment variables
1) Download the forge MDK and your favorite java IDE (eclipse or Intellij Idea will have the most support)
2) Think of a modid for your mod, e.g. "yourmod"
3) open up build.gradle and src/main/resources/META-INF/mods.toml and change all the references to "examplemod" and "modid" to your modid

If you are using Eclipse:
	4) open a command prompt in your mod folder and run |gradlew eclipse|
	5) Import the MDK into your IDE's workspace
	-- if you're using eclipse, set your workspace to one folder up from your mod folder when you open eclipse,
	-- and then go to File -> Import -> Gradle -> Existing Gradle Project -> your mod folder
	-- if you don't see Existing Gradle Project , download the Buildship plugin from the eclipse marketplace
If you are using Intellij, check the forge MDK's readme for instructions
  
6) Now you're ready to start modding! Check out the examplemod for examples of forge's event system
  -- the idea is that you tell forge to call a specific function that you've defined when a particular thing happens
  ```

## Helpful Things for Getting Started

* [Adding event listeners](https://gist.github.com/Commoble/a60d03e52fb4a38c42ac4fd2a7153b4c)
* [Using EventBusSubscriber and ObjectHolders to register things](https://gist.github.com/Commoble/1fced1e0ccfb3f40f79eaf73e8064b89)
* [Creating generic registry helper methods to make registering things easier](https://gist.github.com/Commoble/d19f1cd597fcfc35d443295f8e3168c0)
* [Creating generic registry helper classes to make registering things easier](https://gist.github.com/Commoble/390caa58390e42d156b3e8ec351b3ccf)
* Using Deferred Registers and RegistryObjects to register things (not done yet)

## Helpful Things for Doing Specific Things

* [Adding event listeners to client-only events](https://gist.github.com/Commoble/ffa5c45e74e77aa7b9e2cc5dbeca2f9f)
* [Saving tile entity data to the hard drive and syncing their data to the client](https://gist.github.com/Commoble/c96271da4d8cf4e33f4370eda952f210)
* [Custom Dimensions and How you Go to Them](https://gist.github.com/Commoble/ac7d7b57c9cbbfcae310c4ab110c3cc0)
* [An example of a loot table that generates random potions](https://gist.github.com/Commoble/96f7eab193bfb08f3e1bff142f5f0c6d)
* [Creating custom loot table functions](https://gist.github.com/Commoble/407716790fc1d3717b1a3eaac29f7423)
* [Generating data jsons in-Java with minecraft's data generators](https://gist.github.com/Commoble/a821e8fe62238c913bd189aaffe7e425)


## Helpful Things that Do Specific Things For You

* [Utility for creating config values and automatically subscribing them to the config load/reload event](https://github.com/Commoble/configexample/tree/master/src/main/java/com/github/commoble/confighelper)
* [Utility for setting up a reload listener to load json assets into java objects](https://gist.github.com/Commoble/2fc5a5f831529767f52d37900844c6ba)
* [Utility for writing a Map into NBT](https://gist.github.com/Commoble/9316f64c4a5bc9474312382872465482)
* [Utility for writing a List into NBT](https://gist.github.com/Commoble/463df511582ef7e8783cacb7e06c9903)


## Helpful Information About Specific Things

* [What's the difference between the different VoxelShape getters in forge for minecraft 1.15?] (https://gist.github.com/Commoble/1e44951973ccc518248ccc0ee3880bf9)