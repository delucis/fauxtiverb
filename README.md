# fauxtiverb [![Build Status](https://travis-ci.org/delucis/fauxtiverb.svg)](https://travis-ci.org/delucis/fauxtiverb) [![GitHub release](https://img.shields.io/github/release/delucis/fauxtiverb.svg?maxAge=600)](https://github.com/delucis/fauxtiverb/releases/latest)

Friendly impulse response reverb in Max/MSP with [HISSTools](https://github.com/HISSTools/HISSTools_Impulse_Response_Toolbox)’s `multiconvolve~`.

## Installation

1. Download the [__latest version__](https://github.com/delucis/fauxtiverb/releases/latest) (click on `fauxtiverb.zip`).

2. Unzip it to your packages directory:
`~/Documents/Max/Packages` for Max 6 or `~/Documents/Max 7/Packages` for Max 7.

3. In Max, open `fauxtiverb` in the Package Manager for more information.

## Usage

`fauxtiverb` contains three modules that convolve audio input with impulse responses to create a reverb effect:

- `fauxtiverb-m2m~` — a mono-to-mono convolution module [CPU×1]
- `fauxtiverb-m2s~` — a mono-to-stereo convolution module [CPU×2]
- `fauxtiverb-s2s~` — a stereo-to-stereo convolution module [CPU×4]

Each module has a built-in graphical interface when loaded in a `bpatcher` object, but can also be used as a normal object and adressed with messages. See the module help files for more details.

## Acknowledgments

This package depends on the `multiconvolve~` external from [Alex Harker](http://www.alexanderjharker.co.uk/) and [Pierre Alexandre Tremblay](http://www.pierrealexandretremblay.com/)’s [HISSTools](https://github.com/HISSTools/HISSTools_Impulse_Response_Toolbox).

## License

The HISSTools, including the `multiconvolve~` external, are Copyright © 2012 Alex Harker and Pierre Alexandre Tremblay and are distributed under a [3-Clause BSD License](https://opensource.org/licenses/BSD-3-Clause).

The `fauxtiverb` package is distributed under a [3-Clause BSD License](https://opensource.org/licenses/BSD-3-Clause).
