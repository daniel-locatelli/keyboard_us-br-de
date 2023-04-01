<!-- #######  HEY, I AM THE SOURCE EDITOR! #########-->
<h1>Polyglot Keyboard Layout for Windows</h1>
<p>US ANSI keyboard layout converted to accept Portuguese and German special characters.</p>
<h3>It uses <a href="https://en.wikipedia.org/wiki/Dead_key">dead keys</a> to include:</h3>
<p>&atilde; &ntilde; &otilde; &Atilde; &Ntilde; &Otilde; &acirc; &ecirc; &icirc; &ocirc; &ucirc; &Acirc; &Ecirc; &Icirc; &Ocirc; &Ucirc; &aacute; &eacute; &iacute; &oacute; &uacute; &yacute; &Aacute; &Eacute; &Iacute; &Oacute; &Uacute; &Yacute; &agrave; &egrave; &igrave; &ograve; &ugrave; &Agrave; &Egrave; &Igrave; &Ograve; &Ugrave; &auml; &euml; &iuml; &ouml; &uuml; &yuml; &Auml; &Euml; &Iuml; &Ouml; &Uuml; &Yuml; ç Ç &sup1; &sup2; &sup3; ⁴ ⁵ ⁶ ⁷ ⁸ ⁹ ⁰ &ne; &Sigma; &euro; &ordm; &ordf; &szlig; &deg; &le; &ge; ₁ ₂ ₃ ₄ ₅ ₆ ₇ ₈ ₉ ₀ &asymp; &sect;</p>

<h3><br />Layout base</h3>

![US-BR-DE](https://user-images.githubusercontent.com/15069239/229212255-5c38a18c-41e2-410a-a29d-4f6f25439ccb.jpg)


<h3><br />Layout Shift</h3>

![US-BR-DEShft](https://user-images.githubusercontent.com/15069239/229212303-c9859f00-33d8-4cd6-a2a7-47bcb3bfe6b4.jpg)


<h3><br />Layout ALTGR</h3>

![US-BR-DEAltGr](https://user-images.githubusercontent.com/15069239/229212329-81509465-ccb5-4dde-a507-35b00e00b8f8.jpg)


<h3><br />Layout Shift + ALTGR</h3>

![US-BR-DEShftAltGr](https://user-images.githubusercontent.com/15069239/229212377-24dbdde8-ee25-4b65-8fc7-d00ffae62354.jpg)


<p>&nbsp;</p>

<h2>Tools used</h2>
<p>This was developed on Microsoft Keyboard Layout Creator <a href="https://www.microsoft.com/en-us/download/details.aspx?id=102134">MKLC 1.4</a>
</br>You can learn how to use the MKLC 1.4 here: https://www.youtube.com/watch?v=HMDSJfwi0Kc
</br>It was useful to look at this digital <a href="https://learn.microsoft.com/en-us/globalization/keyboards/kbdbr_2">Brazilian ABNT2 layout</a> and the <a href="https://learn.microsoft.com/en-us/globalization/keyboards/kbdgr">German layout</a>
</br>I am currently using the Keyboard <a href="https://www.keychron.com/pages/keychron-k6-pro">Keychron K6 Pro</a> which can be further customized with QMK &amp; VIA, however the layout should work in any US ANSI layout<br /><a href="https://qmk.fm/">QMK Firmware</a><br /><a href="https://www.caniusevia.com/">VIA</a></p>

<h2>Installation</h2>

![Tutorial01](https://user-images.githubusercontent.com/15069239/229212620-375279e6-5e2b-4795-a0fd-cbbcd7cc35c0.jpg)


![Tutorial02](https://user-images.githubusercontent.com/15069239/229212632-1d79d91e-52c5-43e0-bb84-183344144971.jpg)


![Tutorial03](https://user-images.githubusercontent.com/15069239/229212651-be84f442-a285-43fa-a5de-a84c64d004db.jpg)


![Tutorial04](https://user-images.githubusercontent.com/15069239/229212661-8f005a13-51d1-46a8-b0cb-8de35f2e26eb.jpg)


![Tutorial05-trim](https://user-images.githubusercontent.com/15069239/229213347-fe9fad6f-69b8-460d-bdbb-6e19949b9b9e.jpg)


![Tutorial06-trim](https://user-images.githubusercontent.com/15069239/229213373-3bd79d17-53c4-42c0-957a-4ee66827a6e8.jpg)


![Tutorial07-trim](https://user-images.githubusercontent.com/15069239/229213449-469e2e8e-6788-4c7c-ba39-37577b7989fa.jpg)


![Tutorial08-trim](https://user-images.githubusercontent.com/15069239/229213477-b5add394-75df-41d0-8d4c-5d1856b699e0.jpg)


![Tutorial09](https://user-images.githubusercontent.com/15069239/229212778-f2a1cc3d-13a3-450d-bd9c-29c23b70b00f.jpg)


<h2><br />How I got to this setup</h2>

<h3>VIA</a></h3>
<p>https://www.caniusevia.com/</p>
<p>Initially, I tried to customize everything using the VIA website.<br />However it was quite basic, there was no option to add these custom Brazilian/German letters.<br />As it is based on the QMK firmware, I went to this page https://docs.qmk.fm/#/keycodes and tried to find a code to use on the VIA configurator.<br />I even tried to use a macro trick to get to ALT + XXXX https://en.wikipedia.org/wiki/Alt_code <br />As nothing worked, I moved to the QMK firmware.</p>

<h3>QMK Firmware</a></h3>
<p>https://qmk.fm/</p>
<p>This tool is quite powerful, you can customize almost everything on your keyboard.
<br />First I managed to clone the Keychron K6 Pro repository. Which was a pain, because their <a href="https://github.com/Keychron/qmk_firmware/tree/bluetooth_playground">Bluetooth repository</a> is not on the same branch as the rest of QMK Firmware.
<br />Initially I downloaded the whole repository with all available keyboard firmware (1GB+). Then I learned how to download just a repository branch (thanks ChatGPT).<br />This firmware is based in the C language, for that, you have to either install the MSYS or their QMK_MSYS, which in this case makes things a bit easier.<br />Updating the keyboard functions was quite easy, I just had to edit the "keymap.c". I also used their <a href="https://docs.qmk.fm/#/reference_keymap_extras">language-specific Keycodes</a>.<br />After that, I changed the keyboard to access the special character I wanted and flashed the firmware.<br />After all that I finally discovered that it doesn't matter how the firmware is configured if the windows language input is not configured properly.<br />It means that I would have to alternate the language input between US, ABNT2, and DE in the taskbar, which is exactly what I was trying to avoid.</p>
<h2>Conclusions</h2>
<ul>
<li>MKLC 1.4 is quite basic but does the work of merging different languages.</li>
<li>VIA should be used to create simple shortcuts and macros.</li>
<li>QMK can be used for everything else (really, the sky is the limit there).</li>
</ul>
