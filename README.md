# Python development for Glyphs.app

These are text editor snippets intended to facilitate Python (both 2 and 3) development for Glyphs.app. Have fun. 

**TextMate:** Since I use TextMate myself, the TextMate snippets can safely be assumed to be up to date most of the time. 

**Sublime Text:** Newer versions of Sublime Text can read TextMate bundles, so you are up to date automatically. See installation instructions below.

**Atom:** Since I don’t use Atom, I depend on other people’s pull requests. Hence, the Atom snippets are usually out of date. If you want up-to-date snippets for Atom, feel free to contribute to this repository on a regular basis.

### Snippets

* `gspy⇥` Basic structure of a Glyphs script that iterates through selected layers.
* `title⇥` MenuTitle (name of the script as it appears in the *Script* menu) and docstring (text for the tooltip).
* `clear⇥` Clears the Macro Window log.
* `macro⇥` Clears the Macro Window log and brings the Macro Window to the front.
* `angle⇥` Function returning the angle between two points.
* `center⇥` Convenience function returning the center (as NSPoint) of an NSRect.
* `circle⇥` Function returning a GSPath containing a circle.
* `otclass⇥` Function that creates or (if it already exists) updates an OpenType class.
* `otfeature⇥` Function that creates or (if it already exists) updates an OpenType feature.
* `italic⇥` Function that returns a point position that respects an italic angle.
* `offset⇥` Function that offsets a GSLayer.
* `round⇥` Function that rounds the corners of a GSLayer.
* `measurement⇥` Function that returns intersection points (like the Measurement tool does) of the decomposed and overlap-removed layer.
* `msg⇥` Function for displaying a simple (non-Vanilla) message dialog.
* `select⇥` Adds item on a layer to the user selection.
* `tab⇥` Opens a new tab with supplied text or collection of layers.
* `transform⇥` Function for creating a NSAffineTransform object, necessary for shifting, scaling, skewing, rotating.
* `bezier⇥` Function for returning the x,y for a given t on a cubic Bézier curve segment.
* `clipboard⇥` Function for setting the clipboard.
* `random⇥` Import the *random* library, seed, and create a random integer.
* `sort⇥` Sort a list of objects by a certain attribute of those objects (e.g. layers by their max y).
* `terminal⇥` Execute a Terminal (bash) command.
* `trace⇥` Import the *traceback* library and print a traceback. Useful for *except* clauses.
* `subtract⇥` Subtract GSPath objects.
* `intersect⇥` Intersect GSPath objects.
* `timer⇥` Method for taking and reporting elapsed time.
* `notification⇥` Display a floating notification in top right corner of screen.
* `write⇥` Method *saveFileInLocation()* for writing UTF-8 string into a new file.
* `keys⇥` NSEvent algorithm for determining which modifier keys are pressed by the user.
* `g23⇥` A try/except clause for compatibility with Glyphs 2 and 3.
* `fut⇥` The *from future* imports for Glyphs 2/3 and Python 2/3 compatibility.

#### Vanilla-specific snippets

* `gsgui⇥` Basic structure of a Glyphs script with a dialog (GUI). Uses Vanilla.
* `pref⇥` Register, load, register & load, or save preferences for Vanilla GUI items.
* `button⇥` Vanilla popup and square button.
* `text⇥` Vanilla text box or text edit field.
* `checkbox⇥` Vanilla checkbox.
* `radio⇥` Vanilla radiobuttons.
* `progress⇥` Vanilla progress bar.
* `tooltip⇥` Tooltip for a Vanilla object.
* `vanilla⇥` Show help for Vanilla classes.

#### Plugin SDK-specific snippets

* `dec⇥` Decorators.
* `rgb⇥` NSColor object with RGB definition.
* `plugindef⇥` Function definition structure better suited for the [Plugin SDK](https://github.com/schriftgestalt/GlyphsSDK/).
* `log⇥` Log a message to the console.
* `url⇥` Prefill the *productPageURL* or *updateFeedURL* entry of a plug-in’s *Info.plist* with a GitHub URL.
* `key⇥` Dedine a keyboard shortcut for a plug-in, including the modifier keys.
* `cond⇥` Inserts the `conditionsAreMetForDrawing()` method for [Reporter plug-ins](https://github.com/schriftgestalt/GlyphsSDK/tree/master/Python%20Templates/Reporter). It will return `False` if the user is in text mode or switched to the Hand tool (H).

### Installation

* TextMate bundle: double click to install
* Sublime Text: Open *Sublime Text > Preferences > Browse Packages…* and move the `Python for Glyphs.tmbundle` into the folder that appears
* Atom: move to `~/.atom/packages/python-to-glyphs`

### License

Copyright 2014 Rainer Erich Scheichelbauer (@mekkablue).
Some code by Georg Seifert (@schriftgestalt). Atom adaptation by Kenneth Ormandy (@kennethormandy).

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

See the License file included in this repository for further details.
