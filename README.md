﻿# Read this first.
Original version of this [book](https://github.com/horance-liu/tensorflow-internals) was translated semi-automatically with Google translate.
`It may and will contain typos in text, code and comments`. It needs careful proof-reading. The source code of this English version is hosted
[here](https://github.com/sergey-serebryakov/tensorflow-internals).

# TensorFlow Internals.

It is an open source eBook about TensorFlow kernel and implementation mechanism, including programming model, computation graph, distributed training for machine learning.

## Downloads

You can obtain full latex source files of TensorFlow Internals from [https://gitlab.com/horance/tensorflow-internals](https://gitlab.com/horance/tensorflow-internals)

## Install Tex

You should install full texlive packages.

- Ubuntu     

```bash
$ sudo apt-get install texlive-full
```

- MacOS

Download [MacTeX.pkg](http://tug.org/mactex/), and install it.

- Windows

Download [CTEX-full](http://www.ctex.org/CTeXDownload), and install it.

## Install Missing Fonts

Then you should install some missing chinese fonts. Please download missing fonts from Gitlab.

```
$ git clone https://gitlab.com/horance/fonts.git
```
Note: `Monaco_Linux.ttf` is not a valid font on Windows, try this: https://github.com/todylu/monaco.ttf

Then install all missing fonts.

- Ubuntu

```bash
$ sudo cp fonts/* /usr/local/share/fonts
$ sudo fc-cache
```

- MacOS

Import all missing fonts into fontbook, then cache all fonts.

```bash
$ sudo fc-cache
```

- Windows

Copy the all missing fonts into C:/WINDOWS/Fonts, then cache all fonts.

```bash
$ fc-cache
```

## Build

```bash
$ make
```

if you happen to Error begin with `?`, then press `R`(not `r`) and `Enter` to continue.

## Preview PDF

- Mac OSX

```bash
$ open output/tensorflow-internals.pdf
```

- Ubuntu

```bash
$ okular output/tensorflow-internals.pdf
```

if no okular installed, please install it.

```bash
$ sudo apt-get install okular
```

- Windows

open the file from directory `tensorflow-internals/output`.

## License

[MIT License](http://opensource.org/licenses/mit-license.html)

## rangerQ's translation notes
- My translation is based on [this version](https://github.com/sergey-serebryakov/tensorflow-internals) made by Google translate. My version includes translation, proofreading, and editing for better readability.

- The deep learning terminologies and acronyms were carefully checked and listed with `\usepackage{glossaries}`. So that changes to the terminologies can be made globally in the `glossaries.tex` file. The glossary list is not necessary for reading, but only for translation optimization. If you have better translation of the terminologies, please edit the `name={}` in `glossaries.tex`. 
