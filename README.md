# Polyglot Keyboard Layout for Windows
Custom US keyboard layout converted to accept Portuguese and German special characters
This was developed on on Microsoft Keyboard Layout Creator (MKLC 1.4) https://www.microsoft.com/en-us/download/details.aspx?id=102134
It was useful to look at this digital Brazilian ABNT2 layout https://learn.microsoft.com/en-us/globalization/keyboards/kbdbr_2
And also the German layout https://learn.microsoft.com/en-us/globalization/keyboards/kbdgr

I am currently using the Keyboard Keychron K6 Pro https://www.keychron.com/pages/keychron-k6-pro
Which can be further customized with QMK & VIA
QMK Firmware https://qmk.fm/
VIA https://www.caniusevia.com/

Layout base
![US-BR-DE](https://user-images.githubusercontent.com/15069239/229187806-0d8ab97b-0b77-48b5-a82b-8f14525c122a.jpg)

Layout Shift
![US-BR-DEShft](https://user-images.githubusercontent.com/15069239/229187934-41299e41-3ed6-4318-872e-fe68c0e4b6fc.jpg)

Layout ALTGR
![US-BR-DEAltGr](https://user-images.githubusercontent.com/15069239/229188048-de15781a-ba96-4156-afd5-a02f38f0b05c.jpg)

Layout Shift + ALTGR
![US-BR-DEShftAltGr](https://user-images.githubusercontent.com/15069239/229188192-72584a1d-2744-475e-8052-2fcdacbfa392.jpg)


How I got to this setup:
VIA Website
Initially I tried to customize everything using the VIA website.
However it was quite basic, there was no option to add these custom brazilian/german letters.
As it is based on the QMK firmware, I entered in this page https://docs.qmk.fm/#/keycodes and tried to find a code to use in the VIA page.
I even tried to use a macro trick to get to ALT + XXXX https://en.wikipedia.org/wiki/Alt_code 
As nothing worked, I moved to the QMK firmware.
QMK Firmware
This tool is quite powerful, you can change almost everything in your keyboard.
So I managed to clone the Keychron K6 Pro repository. Which was a pain, because their bluetooth repository is not on the same branch as the rest of QMK Firmware.
At first I downloaded the whole repository with all available keyboard firmwares (1GB+). Then I learned how to download just a branch of a repository (thanks ChatGPT).
This firmware is based in the C language, for that you have to either install the MSYS or their QMK_MSYS, which make things a bit easier.
Updating the keyboard functions was quite easy, I just had to edit the "keymap.c". I also used their language specific helpers.
After that I changed the keyboard to access the keys I wanted and flashed the firmware.
Afeter all that I finally discovered that it doesn't matter how the firmware is configured if the windows language input is not configured.
It means that I would have to alternate the language input between US, ABNT2 and DE in the task bar. Which is exatcly what I was trying to avoid.

Conclusions
MKLC 1.4 which is quite basic but does the work of merging different languages.
VIA should be used to create simple shortcuts and macros.
QMK can be used for everything else (really, the sky is the limit there).
