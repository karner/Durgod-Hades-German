# Durgod Hades config with macros for German Umlaute
This is a .hera file alongside all macros necessary for typing German Umlaute on Windows and macOS.

Supported are: ä ö ü Ä Ö Ü and ß

Fn2 + corresponding letter will type the lower case character.

e.g.: Fn2 + a -> ä, Fn2 + s -> ß

Fn1 + Fn2 + corresponding letter will type the upper case character.

e.g.: Fn1 + Fn2 + a -> Ä


# How this works
The characters are created using a macro which presses a sequence of keys specific to each platform.
In this hera config, profile 1 holds the macros for Windows, and profile 2 holds the macros for macOS.
I chose a delay of 5 ms between each key action which seems to work well for me, but might need some tweaking on different systems.
Feel free to use the macro files in your own .hera config and assign them to whichever keypress you prefer.

## Windows
The macros use ASCII input by holding the Alt-key while pressing the numpad keys for the corresponding character.

[Alt down] 1 3 2 [Alt up] will result in ä

As far as I know this method is independent of the input variant chosen.

## macOS
The macros use the combination of pressing Alt + u followed by the respective character, or Alt + s for ß.

This method was tested with the standard US keyboard layout, possibly there are differences when using a different layout.

## Known issue
As this uses the numpad, on Windows Numlock needs to be on for this to work properly. If pressing the buttons results in cursor movement or other unexpected behavior which might be related to the numpad acting as cursor keys. The state of numpad on boot can be set in the BIOS, or in the registry editor using the InitialKeyboardIndicators value. Please make sure you know what you do when manipulating registry values. For me setting the value to 2 for all users solved the issue, but watch out, it might be different for you. (Or put differently: You're on your own on this path, as stated below: ...NO LIABILITY FOR ANY CLAIM, DAMAGES...)

# License (MIT)
Copyright 2021 Mathias Karner

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
