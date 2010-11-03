# ImageTweak ![ImageTweak icon](http://github.com/CAFxX/ImageTweak/raw/master/skin/imagetweak32.png)
Mozilla Firefox add-on for improving the image viewing UX 

[Homepage](http://cafxx.strayorange.com/ImageTweak) - 
[Downloads](https://addons.mozilla.org/en-US/firefox/addon/3683) - 
[User guide](https://github.com/CAFxX/ImageTweak/wiki/ImageTweak-user-guide) - 
[Source code (GitHub)](http://github.com/CAFxX/ImageTweak) - 
[Contact me](mailto:imagetweak@cafxx.strayorange.com)

ImageTweak is an add-on for Firefox, Iceweasel and SeaMonkey that enhances the vision of images in the browser by allowing zooming, rotating and viewing them against a custom/neutral/dark/black background.

ImageTweak is free software licensed under the terms of the [GPLv3](http://www.gnu.org/licenses/gpl-3.0-standalone.html).

![GPLv3 logo](http://www.gnu.org/graphics/gplv3-88x31.png)

## User guide
An updated [user guide](https://github.com/CAFxX/ImageTweak/wiki/ImageTweak-user-guide) is available.

## Contribute
You can contribute code to ImageTweak by sending patches or pull requests, a [list of planned features](http://github.com/CAFxX/ImageTweak/wiki) is available. Alternatively you can make donations to support the development of ImageTweak on [addons.mozilla.org](https://addons.mozilla.org/en-US/firefox/addon/3683). 

You can also help by [reporting bugs](http://github.com/CAFxX/ImageTweak/issues) (please, try to be as acccurate as possible by including your OS, browser version, extensions installed, plugins and exact steps to reproduce the bug: if I can't reproduce it, most likely I won't be able to fix it!), [suggesting new features](http://github.com/CAFxX/ImageTweak/wiki) or by [translating ImageTweak in your language](http://www.babelzilla.org/).

## Extension compatibility
Other extensions that wish to play nice with ImageTweak can use the following functions to test for the presence of ImageTweak.

```js
	// Check if ImageTweak is installed and enabled:
	function isImageTweakEnabled() {
		try {
			return ImageTweakHelper.enabled();
		} catch (e) {
			return false;
		}
	}

	// Check if if the document doc is being displayed using ImageTweak
	function isImageTweakDocument(doc) {
		try {
			return ImageTweakHelper.enabledForDocument(doc);
		} catch (e) {
			return false;
		}
	}
```