# PPT timer
! [ppttimer](ppttimer.png)
[Download](https://github.com/old9/ppttimer/releases)

## A simple PowerPoint timer for Windows, built with [Autohotkey] (http://autohotkey.com).
### Key features:
* Countdown timer starts/stops automatically when presentation begins / ends
* Always on top, even in slideshow view, while allowing PowerPoint to be operated normally
* Customizable font, transparency, and more via ini config file
* Standalone timer, can also be set to start / stop manually, independent of PowerPoint

## Sources
- [Yet Another CountDown Script](http://www.autohotkey.com/board/topic/19679-yet-another-countdown-script/)
- [Countdown timer app](http://www.autohotkey.com/board/topic/57463-countdown-timer-app/)。

## Screenshot:

! [Screenshot](screenshot.png)

## How to install and use

No installation required, [download] (https://github.com/old9/ppttimer/releases) and unzip, run ppttimer.exe and you're ready to go.
The PPT will be automatically detected when the program is launched, and the timer will be automatically started once the PPT starts to be shown.
If it is not a PPT projection, other presentation methods such as PDF can also be started manually with shortcut keys.
The default shortcut is set to start the  show 'F12', stop the show 'Ctrl' + 'F12', and exit the program 'Windows). `+`ESC`。

## Ini config:
```ini
[Main]
; The countdown time, in seconds, defaults to 1200 seconds, which is 20 minutes.
Duration=1200

; Advance reminder time, in seconds. The default is 120 seconds, which is 2 minutes.
Ahead=120
; Whether to play a sound and the sound path when you are reminded in advance
PlayWarningSound=1
WarningSoundFile=.\beep.mp3

; When the time is up, whether to play a sound and the sound path
PlayFinishSound=1
FinishSoundFile=.\applause.mp3

; Window style
; transparency
opacity=180
; Window background color
backgroundColor=FFFFAA
; The size of the window, the position is fixed in the upper right corner
width=300
height=70

; Font style
fontface=Microsoft Yahei
fontweight=bold
fontsize=40
textcolor=000000

; Font color for advance reminders
AheadColor=9D1000

; The font color after the timeout
timeoutColor=HT0000

; Key Legend: ^ Ctrl，# Windows，+ Shift，! Alt。
; Start manual timing
startKey=F12
; Stop the timer
stopKey=^F12
; Exit the main program
quitKey=#ESC
```

## Installation instructions
* Go to [Autohotkey Home](https://autohotkey.com) to download Autohotkey and install it.
* Use the built-in compilation and packaging tool 'Compiler\Ahk2Exe.exe' to compile the ahk file.
* Alternatively, you can simply rename the `*.ahk` script file to match the name of the Autohotkey.exe that will run it. By doing so, Autohotkey will automatically load the timer script by default when run.

## Updates
* More controllable parameters
* Automatic detection of windows other than PPT

## licence
Licensed under the MIT.

