# SublimeConcat

Automatically concatenate all of the dependencies in the current file.

## Installation

**Without Git:** Download the latest source from [GitHub](https://github.com/magnobiet/SublimeConcat) and copy the whole directory into the Packages directory.

**With Git:** Clone the repository in your Sublime Text 2 Packages directory, located somewhere in user's "Home" directory:

	git clone git://github.com/magnobiet/SublimeConcat.git


The "Packages" packages directory is located at:

* OSX:

	~/Library/Application\ Support/Sublime\ Text\ 2/Packages/

* Linux:

	~/.Sublime\ Text\ 2/Packages/

* Windows:

	%APPDATA%/Sublime Text 2/Packages/

## Usage

Define the dependencies using the @import syntax

CSS:

	@import url('bootstrap.min.css');

	body {
		background-color: #fff;
	}

JS:

	//@import url('jquery.min.js');

	$(document).ready(function() {
		console.log('ready');
	});

`Ctrl + Shift + C` or `Command + Shift + C` will concatenate all of the dependences into a new file: `{{filename;}}.cat.{{extension;}}`

Use with [YUI Compressor](https://github.com/leon/YUI-Compressor) and [SublimeOnSaveBuild](https://github.com/alexnj/SublimeOnSaveBuild) for automatic concat and minify

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D

## History

Check [HISTORY.md](https://github.com/magnobiet/SublimeConcat/blob/master/HISTORY.md)

## License

[MIT License](http://magno.mit-license.org/)