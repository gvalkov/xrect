xrectsel
========

A rectangle selection tool for X11. 

![Demo](https://raw.githubusercontent.com/gvalkov/xrectsel/master/.demo.gif)

Usage
-----

```
Usage: xrectsel [-hfwsb]

Options:
  -h, --help           show this help message and exit
  -f, --format         output format (default: %x %y %w %h)
  -w, --border-width   set border width (default: 1)
  -s, --border-style   set border line style (default: solid)
  -b, --border-color   set border color (default: white)

Color Format:
  hex: #7CFC00
  rgb: 127,252,0
  x11: Lawn Green

Styles:
  border-style: solid dash double-dash

Format Placeholders:
  %x %X: offset from left/right of screen
  %y %Y: offset from top/bottom of screen
  %w %h: selection width/height

Examples:
  xrectsel -w 3 -b "Lawn Green"
  xrectsel -f "%wx%h+%x+%y\n"
  xrectsel | read x y width height
```

License
-------

Xrectsel is released under the terms of the [Revised BSD License][1].

[1]: https://raw.githubusercontent.com/gvalkov/xrectsel/master/LICENSE
