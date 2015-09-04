Iso Dark Theme for Godot
==============

Iso Dark is a clean, modern dark theme for the  [Godot Engine](http://www.godotengine.org), designed to make games early in development look good, and to be easily modified as a game matures.

<img src="https://raw.githubusercontent.com/GalanCM/Iso-Themes/master/screenshot.png">

#### To support these design goals, Iso Dark is build around the following concepts:
* **Ultra-minimalism:** Results in a clean look, and more importantly is easily modified. Details can be more easily changed without breaking the overall feel. While elements like gradients and shadows can help with the overall presentation of a theme, they would have to be matched, and would limit aesthetic choices during development.
* **Light weight:** Iso Dark focuses on only a few core forms so that they can be easily modified and replaced.
* **Two-tone:** The background is a warm black, and all other elements (with a few unavoidable exceptions) are either white or black, with varying transparency. This way, it should be easy to change a single element without clashing with the rest of the theme, and a simple background change can change the feel of the entire theme.
* **Non-distinctive elements:** Nothing in the theme should stand out too much from other themes players commonly see, and should blend into the game itself. Droid Sans was chosen as the default font for this reason, since in addition to being an attractive font with robust Unicode support, it is common, and looks similar to other common fonts.
* **All assets are availible in their original format:** Iso Dark was designed in [Inkscape](http://www.inkscape.org), an open-source vector graphics progam, and files are availible in both svg and png. This should help with theme modification, so developers don't have to worry about recreating elements to match the theme, but can instead modify the originals.
* **Licensed CC0:** For easier use in game jams. While I would appreciate attribution for the theme, I know how difficult it is to keep track of everything that I do during a jam, and I know how much it helps to not have to *worry* about proper attribution.

### Known Bugs:
Due to bugs in Godot, the follow elements cannot be set in the theme, and have to be set manually in each node that uses them:
* Hslider/Vslider → Grabber Hilite
* Tree → Bg Focus

The image files for these elements can be found in the Iso_Dark/pngs/ folder in the zip archive.

### How to Install
* Download the zip using the button on the right side of the main page.
* Extract the ```Iso_Dark/``` directory to your game's resource folder.
* To use the theme in a given ui node, click the ```Theme``` attribute and ```Load``` to select the file ```Iso_Dark/iso_dark.thm```.
* Any children of the themed node should inherit the theme, as long as their Theme attribute is set to ```<null>```. As such, it's recommended that you attach all ui nodes to a central node, and set the theme from there.

### How to make modifications
A full guide to theme modification is outside of the scope of this readme, but the following should help you get started.
* In the editor, in any scene, you can open the ```iso_dark.thm``` by going to the resources tab and clicking the folder icon.
* Selecting the theme should show you an overview of the them, but it's rather limited, and won't have the correct backround color. If you would like to get a better overview of your changes, there is a scene file, ```Iso_Dark/ui_overview.scn``` in the zip archive. Apply your new theme to the Control node to keep track of changes.
* After loading the theme, elements can be modified in the inspector. If you have used image resources before, this should be fairly straight forward.
* To modify existing elements, you'll want to use [Inkscape](http://www.inkscape.org) to edit the files contained in the ```Iso_Dark/svgs/``` folder. All items are named in the form ```element_attribute.svg```. If you wish to create elements from scratch, feel free to use your program of choice.
* If you can't find an element in the svgs folder, it is probably inherited from another element. Check the inheritance tree in the ```Help``` tab of the editor for guidance. Some inheritance is less clear, and you may have to find a similar looking element to make changes. Sadly, trial and error is your friend in these cases.
