# Yellow Taxi Goes Vroom Dialogue Skipper
To improve accessibility and decrease the risk of RSI when speedrunning Yellow Taxi Goes Vroom, the community has decided to allow an AutoHotKey script that skips dialogue when a customizable key is held.

To be transparent with usage, an overlay is displayed in the top left corner of the screen, and a Window Capture must be added to your scene capturing it.

## Installation
1. Install latest v1 (currently v1.1.37.xx) of AutoHotKey from [https://www.autohotkey.com/](https://www.autohotkey.com/ "https://www.autohotkey.com/")
2. Download the latest release of `YTGVDialogueSkipper.ahk`
3. Double-click the script
4. Select key to hold and Confirm key (or configure using the instructions below)
5. Add a Window Capture source to OBS, with source "YTGV_SkippingOverlay"
6. Right-click on the source, Add Filter -> Color Key -> Color of background
7. Adjust settings until the background is transparent and the text is visible

## Configuration
If you open the `YTGVDialogueSkipper.ahk` script in Notepad, you will find a section marked
```
;;;;;;;;;;;;;;;;;;;;;;;;;
; CONFIGURATION SECTION ;
;;;;;;;;;;;;;;;;;;;;;;;;;
```

In that section, you can adjust:
 - the background color of the overlay window (overlayWindowBackground)
 - the color of the "Skipping..." text (overlayFontColor)
 - the key you want to hold to trigger the skipping script (spamKey)
 - the key you have Confirm bound to in-game (confirmKey)
 - whether the skipper should be toggled or held (toggle: if true, the skipper will be toggled when activated)
 - the speed at which the button is spammed in-game in "cycles (down+up) per second" (spamCPS)

By default, these are:
 - Background:
   - 000000 (Black)
 - Font:
   - ffffff (White)
 - Key to hold: Prompted when launching script
 - Confirm key: Prompted when launching script
 - toggle: true
 - Cycles per second: 10 (Cannot be changed if submitting to the leaderboards)

To find the colors you want, you can use https://color-hex.com/

## Credits
This script was based off the auto-skipper for Death's Door, available here: (https://github.com/Museus/deathsdoor-DialogueSkipper)
