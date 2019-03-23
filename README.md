# RimFlix-Anime-Loops
A few looping animations for use with [RimFlix](https://github.com/ritsu/RimFlix). This should be below RimFlix in the mod order.

## Install
1. Download one of the [releases](https://github.com/ritsu/RimFlix-Anime-Loops/releases) and extract its contents.
2. Move the `RimFlix - Anime Loops` folder to `Steam\steamapps\common\RimWorld\Mods`
3. In RimWorld, go to the **Mods** menu and activate **RimFlix - Anime Loops**.
Make sure this mod is below the RimFlix mod in the load order.

## A note on dimensions
The base dimensions for TV textures in Rimworld is 64 x 64 pixels. Tube televisions are scaled 1x1, Flatscreens are 2x1, and Megascreens are 3x1. The "screen area" within these TVs have slightly different aspect ratios due to margins. Here are the default dimensions for each screen area in RimFlix, along with scaled versions for higher definition textures.

#### Tube Telvision
      79 x  64
     157 x 128
     315 x 256
    
#### Flatscreen Television
     155 x  64
     310 x 128
     620 x 256
    
#### Megascreen Television
     225 x  64
     451 x 128
     902 x 256

If you are creating shows to share with others, it's probably best to create images with 64 or 128 pixel height. 256 pixel height images will take a lot longer to load and consume a lot more memory, and the difference is not really noticeable unless you use a camera mod to zoom in much more than normal.

The files in this repo are 128 pixels in height. 64 pixel and 256 pixel versions are available in [releases](https://github.com/ritsu/RimFlix-Anime-Loops/releases).

## Using this repo as a template
1. Copy the folder structure of this repo. Ignore `.gitignore`, `LICENSE`, `README.md`, and the `Languages` folder.
2. Rename the root folder from `RimFlix - Anime Loops` to a name that represents your shows.
3. Replace images in `Textures/Shows/` with your shows' images.
4. Rename and modify the XML files in `Defs/ShowDefs` with your shows' information. The fields you'll want to change are `defName`, `label`, `description`, `secondsBetweenFrames`, and `texPath`. Also, put the television(s) you want your show to play on in `televisionDefs`. You can specify more multiple televisions, but since each television has different aspect ratios, it will probably look weird if you use one set of images for more than one television.
5. Modify `About/about.xml` with your information, and replace the preview image with your own.
6. Follow the [Install](#install) instructions to install and activate your show, using the files you just created / modified. 

## Uploading to Steam Workshop
Once you have installed your show, which is basically a mod, and tested it to see that it works as expected in game, you can upload it to Steam Workshop by doing the following:

1. In **Options**, turn on **Dev Mode** 
2. In the **Mods** menu, select your mod and click **Upload to Steam Workshop**

Follow the rest of the instructions in game.

