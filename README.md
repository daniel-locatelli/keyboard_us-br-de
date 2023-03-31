<!-- #######  HEY, I AM THE SOURCE EDITOR! #########-->
<h1>Polyglot Keyboard Layout for Windows</h1>
<p>Custom US keyboard layout converted to accept Portuguese and German special characters.</p>
<h3>It uses <a href="https://en.wikipedia.org/wiki/Dead_key">dead keys</a> to include:</h3>
<p>&atilde; &ntilde; &otilde; &Atilde; &Ntilde; &Otilde; &acirc; &ecirc; &icirc; &ocirc; &ucirc; &Acirc; &Ecirc; &Icirc; &Ocirc; &Ucirc; &aacute; &eacute; &iacute; &oacute; &uacute; &yacute; &Aacute; &Eacute; &Iacute; &Oacute; &Uacute; &Yacute; &agrave; &egrave; &igrave; &ograve; &ugrave; &Agrave; &Egrave; &Igrave; &Ograve; &Ugrave; &auml; &euml; &iuml; &ouml; &uuml; &yuml; &Auml; &Euml; &Iuml; &Ouml; &Uuml; &Yuml; &sup1; &sup2; &sup3; ⁴ ⁵ ⁶ ⁷ ⁸ ⁹ ⁰ &ne; &Sigma; &euro; &ordm; &ordf; &szlig; &deg; &le; &ge; ₁ ₂ ₃ ₄ ₅ ₆ ₇ ₈ ₉ ₀ &asymp; &sect;</p>

<h3><br />Layout base</h3>

![US-BR-DE](https://user-images.githubusercontent.com/15069239/229187806-0d8ab97b-0b77-48b5-a82b-8f14525c122a.jpg)

<h3><br />Layout Shift</h3>

![US-BR-DEShft](https://user-images.githubusercontent.com/15069239/229187934-41299e41-3ed6-4318-872e-fe68c0e4b6fc.jpg)

<h3><br />Layout ALTGR</h3>

![US-BR-DEAltGr](https://user-images.githubusercontent.com/15069239/229188048-de15781a-ba96-4156-afd5-a02f38f0b05c.jpg)

<h3><br />Layout Shift + ALTGR</h3>

![US-BR-DEShftAltGr](https://user-images.githubusercontent.com/15069239/229188192-72584a1d-2744-475e-8052-2fcdacbfa392.jpg)

<p>&nbsp;</p>

<h3>Tools used</h3>
<p>This was developed on Microsoft Keyboard Layout Creator <a href="https://www.microsoft.com/en-us/download/details.aspx?id=102134">MKLC 1.4</a>
</br>You can learn how to use the MKLC 1.4 here: which you can learn how to use here: https://www.youtube.com/watch?v=HMDSJfwi0Kc
</br>It was useful to look at this digital <a href="https://learn.microsoft.com/en-us/globalization/keyboards/kbdbr_2">Brazilian ABNT2 layout</a> and the <a href="https://learn.microsoft.com/en-us/globalization/keyboards/kbdgr">German layout</a>
</br>I am currently using the Keyboard <a href="https://www.keychron.com/pages/keychron-k6-pro">Keychron K6 Pro</a> which can be further customized with QMK &amp; VIA<br /><a href="https://qmk.fm/">QMK Firmware</a><br /><a href="https://www.caniusevia.com/">VIA</a></p>

<h2><br />How I got to this setup</h2>

<h3>VIA</a></h3>
<p>https://www.caniusevia.com/</p>
<p>Initially, I tried to customize everything using the VIA website.<br />However it was quite basic, there was no option to add these custom Brazilian/German letters.<br />As it is based on the QMK firmware, I went to this page https://docs.qmk.fm/#/keycodes and tried to find a code to use on the VIA configurator.<br />I even tried to use a macro trick to get to ALT + XXXX https://en.wikipedia.org/wiki/Alt_code <br />As nothing worked, I moved to the QMK firmware.</p>

<h3>QMK Firmware</a></h3>
<p>https://qmk.fm/</p>
<p>This tool is quite powerful, you can customize almost everything on your keyboard.<br />So I managed to clone the Keychron K6 Pro repository. Which was a pain, because their <a href="https://github.com/Keychron/qmk_firmware/tree/bluetooth_playground">Bluetooth repository</a> is not on the same branch as the rest of QMK Firmware.<br />At first, I downloaded the whole repository with all available keyboard firmware (1GB+). Then I learned how to download just a repository branch (thanks ChatGPT).<br />This firmware is based in the C language, for that, you have to either install the MSYS or their QMK_MSYS, which in this case makes things a bit easier.<br />Updating the keyboard functions was quite easy, I just had to edit the "keymap.c". I also used their <a href="https://docs.qmk.fm/#/reference_keymap_extras">language-specific Keycodes</a>.<br />After that, I changed the keyboard to access the special character I wanted and flashed the firmware.<br />After all that I finally discovered that it doesn't matter how the firmware is configured if the windows language input is not configured properly.<br />It means that I would have to alternate the language input between US, ABNT2, and DE in the taskbar, which is exactly what I was trying to avoid.</p>
<h2>Conclusions</h2>
<ul>
<li>MKLC 1.4 is quite basic but does the work of merging different languages.</li>
<li>VIA should be used to create simple shortcuts and macros.</li>
<li>QMK can be used for everything else (really, the sky is the limit there).</li>
</ul>
