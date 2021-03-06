# jetzt

*jetzt* is a speed-reader extension for [chrome](http://google.com/chrome) inspired by [Spritz](http://www.spritzinc.com/).

### Tim Scarfe's Branch

- This version implements an alpha of highlighting the current word (see https://www.youtube.com/watch?v=jebPFbVdmTw). This can be done with `ALT`-`R` (article scraping) and the document will be highlighted in the background. `ALT`-`Z` will bring up a scrolling content window. `ALT`-`X` (selection mode with content highlighting). The old `ALT`-`S` is as it was. A lot more work is needed to clean this up. Because of how I manipulate the underlying document, it can make it render differently :(
- If the word is a commonly used english word and less than 6 chars, I reduce the delay time as a function of how common it is
- Punctuation doesn't influence the pivot
- Punctuation is highlighted
- Punctuation color set by .punctuation in css
- Fixes issue where you get punctuation-only displayed for words i.e. "."
- It also displays single quote wrappings, detects when a single quote should be part of the word and then displays it.
- Improved black colour scheme
- Open dyslexic font (I think this would improve anyone's reading speed)
- h0ru5's local heading code, enabled to work for h1-4 using symbols ^*|>
- h0ru5's local article parsing code (Readibility stle), enabled through `alt`-`a`

### Installation

This is very much beta software so a proper chrome extension package is not currently provided. Instead: clone this repository, then, in chrome, navigate to chrome://extensions , enable developer mode, click "Load unpacked extension..." and select the directory you cloned.

Remember to pull every now and then for bugfixes and new features.

### In This Fork (Tim Scarfe)

- New! Automatically generate a local summary and display that with `alt`-`r` (this was done by h0ru5 I just added the new key stroke as he had an ugly confirm() box)
- Tim Scarfe's preferred visual style
- I have enabled h0ru5s heading display using symbols ^,*,|,> for headings 1->4

### Usage

Control is currently keyboard-only.

- Initiate jetzt by pressing `alt`-`s` and clicking on the block of text you wish to read. Alternatively, select some text before pressing `alt`-`s`.

- Initiate jetzt by pressing `alt`-`a` and it will automatically generate a local "readability" summary and display that instead. This means you don't need to select text in any way.

- Change size with `+`/`-`.

- Go faster/slower with up/down arrow keys.

- Go back/forward a sentence with left/right arrow keys (hold `alt` to navigate by paragraphs).

- Pause with space.

- Close with escape.

- Switch between light/dark themes with `0`




### Online Demo

[Here](http://ds300.github.com/jetzt/)

### Bookmarklet

You can also use it as a bookmarklet by:
- Copying the content of bookmarklet.js
- Manually adding a new bookmark
- Pasting the content into the location field. 

### ToDo

Check out the [ToDo](https://github.com/ds300/jetzt/wiki/ToDo) section of the wiki.

### Feature Requests/Contributions

Feel free to open an issue for anything you would like to see in jetzt. 

I also welcome pull requests of all shapes and sizes. This project is still in heavy flux, though, so if you want to make a big change it might be best to open an issue to check that it's not already being worked on.

### Contributors

- [David Sheldrick](https://github.com/ds300)
- [Gustav Ahlberg](https://github.com/Gyran)
- [Peter Uithoven](https://github.com/peteruithoven)
- [h0ru5](https://github.com/h0ru5)
- [fusillicode](https://github.com/fusillicode)
- [Brian Hanson](https://github.com/brianjhanson)
- [ianzapolsky](https://github.com/ianzapolsky)
- [Martin Butt](https://github.com/martinbutt)

### License

The MIT License (MIT)

Copyright (c) David Sheldrick 2014

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.

### | (• ◡•)| (❍ᴥ❍ʋ)
