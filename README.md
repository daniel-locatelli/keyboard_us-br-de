# Polyglot Keyboard Layout for Windows
US ANSI keyboard layout converted to accept Portuguese and German special characters.

## Description
It uses dead keys to include all the other characters, for example, <kbd>AltGr</kbd> + <kbd>'</kbd> <kbd>a</kbd> will return 'ã'.
</br>More information about dead keys [here](https://en.wikipedia.org/wiki/Dead_key).

### Keys included in this layout
&atilde; &ntilde; &otilde; &Atilde; &Ntilde; &Otilde; &acirc; &ecirc; &icirc; &ocirc; &ucirc; &Acirc; &Ecirc; &Icirc; &Ocirc; &Ucirc; &aacute; &eacute; &iacute; &oacute; &uacute; &yacute; &Aacute; &Eacute; &Iacute; &Oacute; &Uacute; &Yacute; &agrave; &egrave; &igrave; &ograve; &ugrave; &Agrave; &Egrave; &Igrave; &Ograve; &Ugrave;
</br>&auml; &euml; &iuml; &ouml; &uuml; &yuml; &Auml; &Euml; &Iuml; &Ouml; &Uuml; &Yuml; ç Ç &sup1; &sup2; &sup3; ⁴ ⁵ ⁶ ⁷ ⁸ ⁹ ⁰ &ne; &Sigma; &euro; &ordm; &ordf; &szlig; &deg; &le; &ge; ₁ ₂ ₃ ₄ ₅ ₆ ₇ ₈ ₉ ₀ &asymp; &sect;

### Layout base
```
 * ┌───┬───┬───┬───┬───┬───┬───┬───┬───┬───┬───┬───┬───┬───────┐
 * │esc│ 1 │ 2 │ 3 │ 4 │ 5 │ 6 │ 7 │ 8 │ 9 │ 0 │ - │ = │       │
 * ├───┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─────┤
 * │     │ q │ w │ e │ r │ t │ y │ u │ i │ o │ p │ [ │ ] │  \  │
 * ├─────┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴─────┤
 * │      │ a │ s │ d │ f │ g │ h │ j │ k │ l │ ; │ ' │        │
 * ├──────┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴────────┤
 * │        │ z │ x │ c │ v │ b │ n │ m │ , │ . │ / │          │
 * ├────┬───┴┬──┴─┬─┴───┴───┴───┴───┴───┴──┬┴───┼───┴┬────┬────┤
 * │    │    │    │                        │    │    │    │    │
 * └────┴────┴────┴────────────────────────┴────┴────┴────┴────┘
```

### Layout Shift
```
 * ┌───┬───┬───┬───┬───┬───┬───┬───┬───┬───┬───┬───┬───┬───────┐
 * │   │ ! │ @ │ # │ $ │ % │ ^ │ & │ * │ ( │ ) │ _ │ + │       │
 * ├───┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─────┤
 * │     │ Q │ W │ E │ R │ T │ Y │ U │ I │ O │ P │ { │ } │  |  │
 * ├─────┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴─────┤
 * │      │ A │ S │ D │ F │ G │ H │ J │ K │ L │ : │ " │        │
 * ├──────┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴────────┤
 * │        │ Z │ X │ C │ V │ B │ N │ M │ < │ > │ ? │          │
 * ├────┬───┴┬──┴─┬─┴───┴───┴───┴───┴───┴──┬┴───┼───┴┬────┬────┤
 * │    │    │    │                        │    │    │    │    │
 * └────┴────┴────┴────────────────────────┴────┴────┴────┴────┘
```

### Layout AltGr
```
 * ┌───┬───┬───┬───┬───┬───┬───┬───┬───┬───┬───┬───┬───┬───────┐
 * │   │ ¹ │ ² │ ³ │ ⁴ │ ⁵ │ ⁶ │ ⁷ │ ⁸ │ ⁹ │ ⁰ │ ≠ │ Σ │       │
 * ├───┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─────┤
 * │     │   │   │ € │   │   │   │ μ │   │ º │   │   │   │     │
 * ├─────┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴─────┤
 * │      │ ª │ ß │ ° │   │   │   │   │   │   │ ´ │ ~ │        │
 * ├──────┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴────────┤
 * │        │   │   │ ç │   │   │   │   │ ≤ │ ≥ │   │          │
 * ├────┬───┴┬──┴─┬─┴───┴───┴───┴───┴───┴──┬┴───┼───┴┬────┬────┤
 * │    │    │    │                        │    │    │    │    │
 * └────┴────┴────┴────────────────────────┴────┴────┴────┴────┘
```

### Layout Shift + AltGr
```
 * ┌───┬───┬───┬───┬───┬───┬───┬───┬───┬───┬───┬───┬───┬───────┐
 * │   │ ₁ │ ₂ │ ₃ │ ₄ │ ₅ │ ₆ │ ₇ │ ₈ │ ₉ │ ₀ │   │ ≈ │       │
 * ├───┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─────┤
 * │     │   │   │   │   │   │   │   │   │   │   │   │   │     │
 * ├─────┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴─────┤
 * │      │   │ § │   │   │   │   │   │   │   │ ` │ ¨ │        │
 * ├──────┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴────────┤
 * │        │   │   │ Ç │   │   │   │   │   │   │   │          │
 * ├────┬───┴┬──┴─┬─┴───┴───┴───┴───┴───┴──┬┴───┼───┴┬────┬────┤
 * │    │    │    │                        │    │    │    │    │
 * └────┴────┴────┴────────────────────────┴────┴────┴────┴────┘
```

## Tools used
* This was developed on Microsoft Keyboard Layout Creator [MKLC 1.4](https://www.microsoft.com/en-us/download/details.aspx?id=102134).
  * You can learn how to use the MKLC 1.4 [here](https://www.youtube.com/watch?v=HMDSJfwi0Kc).
* It was useful to look at this digital [Brazilian ABNT2 layout](https://learn.microsoft.com/en-us/globalization/keyboards/kbdbr_2) and the [German layout](https://learn.microsoft.com/en-us/globalization/keyboards/kbdgr).
* Keyboard [Keychron K6 Pro](https://www.keychron.com/pages/keychron-k6-pro) which can be customized with QMK &amp; VIA, however the setup should work in any US ANSI layout.

## Installation

<details>

<summary>01 Load keyboard file</summary>

### 01 Load keyboard file

<img src="https://user-images.githubusercontent.com/15069239/229212620-375279e6-5e2b-4795-a0fd-cbbcd7cc35c0.jpg" width="600">

<img src="https://user-images.githubusercontent.com/15069239/229212632-1d79d91e-52c5-43e0-bb84-183344144971.jpg" width="600">

</details>

<details>

<summary>02 Build setup package</summary>

### 02 Build setup package

<img src="https://user-images.githubusercontent.com/15069239/229212651-be84f442-a285-43fa-a5de-a84c64d004db.jpg" width="600">

<img src="https://user-images.githubusercontent.com/15069239/229212661-8f005a13-51d1-46a8-b0cb-8de35f2e26eb.jpg" width="600">

</details>

<details>
<summary>03 Install layout</summary>

### 03 Install layout

<img src="https://user-images.githubusercontent.com/15069239/229213347-fe9fad6f-69b8-460d-bdbb-6e19949b9b9e.jpg" width="600">

</details>

<details>

<summary>04 Select the layout in your language settings</summary>

### 04 Select the layout in your language settings

<img src="https://user-images.githubusercontent.com/15069239/229213373-3bd79d17-53c4-42c0-957a-4ee66827a6e8.jpg" width="600">

<img src="https://user-images.githubusercontent.com/15069239/229213449-469e2e8e-6788-4c7c-ba39-37577b7989fa.jpg" width="600">

<img src="https://user-images.githubusercontent.com/15069239/229213477-b5add394-75df-41d0-8d4c-5d1856b699e0.jpg" width="600">

</details>

<details>

<summary>05 Check if it is available in your task bar</summary>

### 05 Check if it is available in your task bar
<img src="https://user-images.githubusercontent.com/15069239/229212778-f2a1cc3d-13a3-450d-bd9c-29c23b70b00f.jpg" width="300">

</details>

## Uninstalling

If you want to modify the layout but want to keep the same name, then you need to do three things:
* Remove the layout from your language settings
* Uninstall your laguage from the system
* Delete the folder generated for the DLL

Only after these previous steps you will be able to use the same name for the layout, and keep everything nice and clean.

## How I got to this setup

### VIA
[VIA Website](https://www.caniusevia.com/)

Initially, I tried to customize everything using the VIA website. However it was quite basic, there was no option to add these custom Brazilian/German letters. As it is based on the QMK firmware, I went to this page https://docs.qmk.fm/#/keycodes and tried to find a code to use on the VIA configurator. I even tried to use a macro trick to get to [ALT code](https://en.wikipedia.org/wiki/Alt_code). 
</br>As nothing worked, I moved on to the QMK firmware.

### QMK Firmware
[QMK Firmware Website](https://qmk.fm/)

This tool is quite powerful, you can customize almost everything on your keyboard.
First I managed to clone the Keychron K6 Pro repository. Which was a pain, because their [Bluetooth repository](https://github.com/Keychron/qmk_firmware/tree/bluetooth_playground) is not on the same branch as the rest of QMK Firmware. Initially I downloaded the whole repository with all available keyboard firmware (1GB+). Then I learned how to download just a repository branch (thanks ChatGPT). This firmware is based in the C language, for that, you have to either install the MSYS or their QMK_MSYS, which in this case makes things a bit easier. Updating the keyboard functions was quite easy, I just had to edit the "keymap.c". I also used their [language-specific Keycodes](https://docs.qmk.fm/#/reference_keymap_extras). After that, I changed the keyboard to access the special character I wanted and flashed the firmware. After all that I finally discovered that it doesn't matter how the firmware is configured if the windows language input is not configured properly. It means that I would have to alternate the language input between US, ABNT2, and DE in the taskbar, which is exactly what I was trying to avoid.

### Conclusions

* MKLC 1.4 is quite basic but does the work of merging different layout languages.
* VIA should be used to create simple shortcuts and macros.
* QMK can be used for everything else (really, the sky is the limit there).
