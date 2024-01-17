# Flash Sprite Sheet Importer

A [Unity](https://unity.com/) plugin to help import Sprite Sheets generated from [Adobe Animate (Flash)](https://www.adobe.com/products/animate.html)

Version 1.2.0 can be installed from this [GitHub Link](https://github.com/JonathanTremblay/FlashSpriteSheetImporter.git)

Older version available on the [Unity Asset Store](https://assetstore.unity.com/packages/tools/sprite-management/flash-sprite-sheet-importer-53520)

## Getting Started

Adobe Animate Instructions
* Each sprite sheet can contain one or more movieclips.
* Export sprite sheets with their corresponding XML files (describing the location of all sprites).
* The Starling XML format now adds the possibility to use pivots from original movieclips.

Unity Instructions
* Get importer window by opening: Window -> Sprite Sheet Importer
* Then select a 2D Texture sprite sheet (alongside accompanying XML file).
* The Force Overwrite Pivot checkbox:
    * Shows a pull down menu to manually select a pivot position.
    * Can be used to ignore existing pivot data from the XML file.
    * Avoid using this option if the pivot point from Animate is already correct!
* The Generate Animation checkbox:
    * Creates an Animator for the sprite sheet.
    * Also creates Animations for each animation movieclip.
    * Shows a field to choose frames per second for those Animations.
    * Shows a Generate GameObject checkbox which can be used to create a GameObject with the Animator.
    * Warning: This function can overwrite previously generated elements without notice.
* Finally, press 'Import Sprites'.

For more details check out the [video on Youtube](https://www.youtube.com/watch?v=zcgmO7sWdWk)

## Compatibility

* Currently support Starling & SparrowV2 sprite sheet formats
* Tested on Windows and Mac with Unity version 2022.3.17 (LTS).

## Known Issues

* None, but issues can be reported on [GitHub](https://github.com/JonathanTremblay/FlashSpriteSheetImporter/issues)

# Credits #

* This tool was created by James Prankard.
* The Whitespace Trimming, XML Pivot and Package implementation were added by Jonathan Tremblay (Cegep de Saint-Jerome).

## Version History

* 1.2.0
    * Updated code for Unity 2021.2+ compatibility. Converted to a package. Excluded files from the Git repository to allow direct installation of the package from GitHub. Jan 17, 2024
* 1.1.1
    * Made animation controller generation optional. Added bug fix for negative (invalid) texture sizes. Apr 1, 2020
* 1.0.6
    * Changed import technique for Unity 2019.1+ compatibility. Jan 15, 2020
* 1.0.5
    * Added update for animation clip generation. Mar 24, 2019
* 1.0.4
    * Added support for empty frames. Mar 21, 2019
* 1.0.3
    * Added MovieClip Alignment and XML Pivot functions. Mar 2, 2019
* 1.0.2
    * Added custom pivot in sprites. Oct 20, 2017
* 1.0.1
    * Original release. Jan 21, 2016