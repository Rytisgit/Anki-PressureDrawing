# Anki-StylusDraw
Initially based on the Anki-TouchScreen addon, updated ui and added pressure pen/stylus capabilities, perfect freehand(line smoothing) and calligrapher functionality.

Website to test the drawing functionality: https://rytisgit.github.io/Anki-StylusDraw/

 <a href="https://rytisgit.github.io/Anki-StylusDraw/">
    <img alt="Draw Demonstration" src="docs/kanjiNewUI.gif" width="75%">
  </a><br>

# Changes
* Added toolbar location configuration and other small fixes.
* Fixed "resize not defined" error. Thanks huandney.
* Updated UI, add option to convert dots, hide cursor and ui while drawing. Thanks rin-w
* Added Perfect Freehand mode(https://github.com/steveruizok/perfect-freehand)
* Added Calligrapher mode(https://github.com/atomanyih/Calligrapher)
* Added pressure sensitivity
* Increased drawing speed
* Added <kbd>,</kbd> for showing/hiding, <kbd>.</kbd> for clearing, <kbd>alt + c</kbd> for calligrapher mode and <kbd>alt + x</kbd> for perfect freehand mode
* Added standalone website to test drawing
* Work around a Windows Pen bug which makes 2 primary pointers appear when drawing in Anki

## Hardware
Tested to work with a Huion H1161, Windows Pen enabled.
### For best exprience dont use software rendering and turn on use pen as a mouse
https://docs.ankiweb.net/platform/windows/display-issues.html
#### Run `echo auto > %APPDATA%\Anki2\gldriver6` in cmd for Qt6
<table> <img alt="Switch away from Software in Qt6" src="docs/qt6fast.png"><tr>
<td> Qt5 rendering change <img alt="Switch away from Software in Qt5" src="docs/dontUseSoftwareRendering.png"> </td>
<td> <img alt="Check use pen as mouse in Windows pen settings" src="docs/usePenAsMouse.png"> </td>
</tr></table>

# Old Description
  
Implements same drawing/writing mechanism as in AnkiDroid. Your writing is NOT intended to remain on the cards after review - same as in AnkiDroid.

Use the menu `View` → `TouchScreen` to activate/change settings.

Use <kbd>Ctrl</kbd> + <kbd>R</kbd> to toggle the touchscreen.

Use icons which will show up in the top right corner of the review screen to temporarily hide/clean the board.
Enjoy!

Warning: the version for Anki 2.0 has limited functionality, and may sometimes not work as expected; since the release of Anki 2.1, the old version is not supported.


#### Changelog:
- 0.2.6 - make "undo" action available under <kbd>Alt</kbd> + <kbd>Z</kbd>
- 0.2.4 - add support for enhanced image occlusion, add a fix for "a double click bug" by LaucianK 
- 0.2.3 - bug fix release, improvements to undo button, styling and performance
- 0.2.1 - minor fix for the buttons/canvas positioning
- 0.2 - added "undo" option, improved the support of long cards plus other minor improvements

#### Disclaimer
Important parts of Javascript code were inspired by <a href="http://creativejs.com/tutorials/painting-with-pixels/index.html" rel="nofollow">creativejs tutorial</a>. I recommend you check out the resource if you are interested in learning JS.

This add-on works well with <a href="https://ankiweb.net/shared/info/1496166067">Anki Night Mode</a>.

#### For developers
You are more than welcome to contribute! While I may not be able to support every user of this addon, I will do my best to help any developer willing to open PR implementing new features or fixing bugs.
