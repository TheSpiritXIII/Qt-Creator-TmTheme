# Qt Creator TmTheme
This project aims to provide a tool for converting TmTheme files to Qt Creator Themes files.

## Usage
Run the Python 3 script on the file you want to convert and also the output location:
```
python converter.py input.tmTheme output.xml
```

Files must be placed in a specific location for Qt Creator to pick them up: These are:

| OS      | Location                              |
| --------|---------------------------------------|
| Windows | ???                                   |
| Linux   | ~/.config/QtProject/qtcreator/styles/ |
| macOS   | ???                                   |

Of course, you may use these locations in the Python script for output.

## Pre-converted Themes
This repository also conveniently ships with several popular themes that have been pre-converted.

In alphabetical order:
 - **One Dark** (Default Atom theme)
 - **Monokai** (Default Sublime Text theme)

It also includes a sample Qt Creator theme file, for reference, named `sample.xml`.

## Screenshots
Because screenshots are bolder than text:
![One Dark](/screenshots/One%20Dark.png?raw=true)
![Monokai](/screenshots/Monokai.png?raw=true)

## Limitations
There are discrepencies between what Qt Creator can highlight and what TmTheme can highlight.

Several differences may arise between what is highlighted. These include, but not limted to:
 - Qt Creator does not seem to like XML comments. Metadata (ie. author name) is unfortunately lost.
 - Qt Creator highlights the `include` keyword the same as it highlights uses of macros.

## Contributing
This project is still in very early development.

Please report any inconsistencies in the GitHub bug tracker. 
