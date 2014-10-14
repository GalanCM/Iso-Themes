Iso Dark Theme for Godot
==============

Iso Dark is an open theme for the  [Godot Engine](http://www.godotengine.org), designed to be used for newly created games, in place of the default theme. It is intended for use in prototypes and game jam games, and it simple enough to be easily modified base for custom game themes.

While the theme that comes with Godot is servicable, and indeed handles the editor quite well, it is a bit heavy, visually, for use in games. Between the strong bevels and the purple base, the theme looks like "The Godot Theme", rather than "My Game's Theme", and it is difficult to change individual elements without changing the whole thing. There is work ongoing to create a [new default theme](https://github.com/okamstudio/godot/pull/704) for the editor, but is still looks more like a theme for an application than a game.

In order to create a good base theme for game, three main goals need to be achieved:

Firstly, the theme must be clean and intuitive. In my mind, these are the two things that make a theme 'beautiful'. Form must follow function, in order for the player to be able to use it effectively, and to do that, extraneous elements should be removed in order to not distract the player. Whether or not a theme succeed or not is subjective, but I believe the new default Godot theme appears to have done this, and I hope that Iso Dark is able to manage this as well.

Secondly, a general-purpose game theme should look good in virtually any game, without the need for heavy modification. It should slip into the background of the game, and not contain elements that would clash heavily against any genre or art style. In reality, this may be impossible to do, but Iso Dark strives for it.

Finally, while a generic theme is good for prototype and game jams, no theme is going to work for every game, and most game developer are going to eventually want their games to have their own identities. To facilitate this, a theme should be easily modifiable, and in fact this may be Iso Dark's greatest strength, as a new skin could be as simple as adding a new background or changing the font, and all asset are open source, making more complex modifications easier. In addition there are plans for an Iso Light theme, for use in games that demand a lighter appearance

To support these goals, Iso is build around the following concepts:
* Ultra-minimalism: Results a clean look, and more importantly is easily modified. Details can be more easily changed without breaking the overall feel, and elements like gradients and shadows don't have to be matched
* Light weight: Iso Dark focuses on only a few core shapes so that they can be more easily replaced.
* Two-tone: The background is a warm black, and all other elements (with a few unavoidable exceptions) are either white or black, with varying transparency. This way, changing a single element shouldn't result in color clashes, and a simple background change should allow for effects throughout the theme.
* Non-distinctive elements: Nothing in the theme should stand out to much from other themes players commonly see, and should blend into the game itself. Droid Sans was chosen as the default font for this reason, since in addition to being an attractive for with robust Unicode support, it is about as indistinct a font as can be found.
* All assets are availible in their original format: This should help with theme modification, so developers don't have to worry about recreating elements to match the theme, but can instead modify the originals.
* CC0: For easier use in game jams. While I would appreciate attribution for the theme, I know how difficult it is to keep track of everything that I do during a jam, and I know how much it helps to not have to worry about proper attribution.
