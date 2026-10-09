<p align="center">
  <a href="README.md"><img src="graphics/flags/gb.png" alt="English" title="English" width="40" height="27"></a>&nbsp;
  <a href="README.uk.md"><img src="graphics/flags/ua.png" alt="Українська" title="Українська" width="40" height="27"></a>&nbsp;
  <a href="README.ru.md"><img src="graphics/flags/ru.png" alt="Русский" title="Русский" width="40" height="27"></a>
</p>

---

# What Is LLX - Narn

<p align="center">
  <a href="LICENSE.md"><img src="https://img.shields.io/badge/license-MIT-blue" alt="License"></a>&nbsp;
  <a href="#"><img src="https://img.shields.io/badge/Android-14%2B-brightgreen" alt="Android"></a>&nbsp;
  <a href="#"><img src="https://img.shields.io/badge/localization-multilingual-green" alt="Localization"></a>
</p>

**LLX** - **Narn** is an actively developed fork of the classic Android launcher **Lightning Launcher** by [Pierre Hebert](https://github.com/pierrehebert/LightningLauncher), updated for modern versions of Android. Pierre built a one-of-a-kind mobile interface where every element, its behavior, size, rotation angle, and font can be customized individually. You get total freedom of layout with no grid restrictions, containers nested inside containers as deep as you like, folders, scripts on any desktop object, and live wallpapers as part of your desktop. The original had all of this back in 2012, and today's shells still can't do half as much.

**LLX** - **Narn** is not just another Android launcher (shell). It's an incredibly fast, compact, and wildly flexible customization tool with **unlimited possibilities** (e**X**treme) for building the **PERFECT home screen** on your phone, tablet, Android TV, and/or Android TV box. And it all works without Google Play Services. **LLX** - **Narn** has only **one limit**: **your imagination**! You're no longer stuck with pages. Your desktop is now a work of art on an endless canvas. The possibilities are limitless.

## Key Features

- separate layouts and grid sizes for portrait and landscape orientation
- scrolling panels and desktops can open on top of the current page
- the ability to pin items so they don't move around
- a settings window to customize the background color, borders, and margins of any element
- "Free mode": a grid? Why bother? Free mode frees you from grid placement and lets you rotate items
- a configurable desktop grid (for fans of the standard layout)
- 22 different gestures can trigger 29 different actions (these actions can also be run through shortcuts)
- use one of your desktops as a lock screen!
- stop points: tell it where scrolling should stop
- configurable scroll direction
- full control over every element, including:
    - choosing the text font, its shadow, and color
    - picking an icon from the gallery, plus its scale and inner scale
    - choosing how the icon and title are positioned relative to each other
    - customizing borders and padding. You can use a .9.png as a background (heads up: this is really cool)
    - adjusting transparency and gesture direction for any action (for example, swiping up on the Chrome icon can launch the Dolphin browser)
- saving your customized desktops as a backup or as a style
- exporting your setup to an APK app
- **LLX** - **Narn** supports a transparent status bar and navigation bar

**LLX** - **Narn** is one of the most customizable launchers out there, which means it might not be the easiest to learn. Like most serious tools, **LLX** - **Narn** takes some time to get the hang of. But isn't that a small price to pay for the most incredible, truly unique home screen among all those identical Android phones?

## Why LLX - Narn Exists

The problem is time. Android kept changing its APIs while the launcher stood still. The original Lightning Launcher by Pierre Hebert hasn't been updated in years. In 2022, Pierre Hebert stepped away from the project... The last active community fork also dates back to 2022, and even then it was behind the Android of its day. Today, on my device (Android 17, One UI 9), the original either refused to launch at all or crashed. What got lost was exactly what users love about it: speed, minimalism, and the feeling that the phone is **REALLY** yours! I kept feeling a sense of loss, like the time of the **LEGEND** was over... and I'd have to settle for the manufacturer's launcher or some other "custom" Android launcher that wouldn't give me even a third of what Lightning Launcher gave me!

**LLX** - **Narn** continues the `developer` branch of the community fork [TrianguloY/LightningLauncher](https://github.com/TrianguloY/LightningLauncher). TrianguloY's fork adapts the original [Lightning Launcher](https://github.com/pierrehebert/LightningLauncher/tree/master) by Pierre Hebert to the Android versions of its time, without digging deep into the existing code. **LLX** - **Narn** runs on the same logic as the earlier versions, with one difference: it takes the next big step. Instead of partially adapting to current Android, it fully uses everything modern versions of the system offer on new chipsets. My goal is to fix everything that crashed, sat broken, didn't work, or only kind of worked, and to add what the original Lightning Launcher was missing, all while keeping the launcher just as light and fast. In short, I preserved the revolutionary 2012 concept and made it possible to run it in 2026 and beyond.

### What Is Narn?

I bet you're curious what **Narn** is all about...! Here's the answer: a long time ago, back when I was young, there was a sci-fi series on TV: [Babylon 5](https://www.imdb.com/title/tt0105946) <details>... Babylon 5 poster ...</details> One of its main characters was named Dgikar, just like me... Yep! I know, his name is spelled differently than mine...! G'Kar. But...! <details>... Photo of Dgikar ...</details>. He belongs to the Narn race, who lived on the planet Narn, which the Centauri (members of another interstellar civilization) nearly destroyed with an asteroid bombardment. So Narn is a tribute to the memory of the planet where my favorite character from my youth was born, and a reminder to everyone:&nbsp;<img src="graphics/flags/russian.png" alt="RU" width="20">&nbsp;war&nbsp;<img src="graphics/flags/ukrainian.png" alt="UA" width="20">&nbsp;never brings anything good!

---

# What's New Compared to Previous Forks

## Runs on Modern Android (14+)

- targetSdk 34; fixed the crashes that showed up on Android 14+: mandatory `RECEIVER_EXPORTED` flags for all `registerReceiver` calls, `FLAG_IMMUTABLE` for `PendingIntent`, and an explicitly declared `foregroundServiceType` for the overlay service
- 16 KB memory page alignment in the native `libll.so` library, a requirement for new 64-bit chipsets on Android 15+
- edge-to-edge layout: real window insets and system bars with no black stripes
- Android 11+ package visibility permissions (`<queries>`, `QUERY_ALL_PACKAGES`)
- removed deprecated APIs that were dropped from newer Android versions (`Canvas.MATRIX_SAVE_FLAG` and others)
- the external lsvg library (from the now-closed JCenter) was restored and built into the code, so the build no longer depends on vanished repositories

## Languages

- **28 languages built into the APK** with no external "language packs" (the old mechanism doesn't work on newer Android)
<details>
<summary><b>Full list of all 28 languages in <b>LLX</b> - <b>Narn</b></b></summary>
<img src="graphics/flags/arabic.png" width="20"> Arabic&nbsp;·&nbsp;<img src="graphics/flags/english.png" width="20"> English&nbsp;·&nbsp;<img src="graphics/flags/bulgarian.png" width="20"> Bulgarian&nbsp;·&nbsp;<img src="graphics/flags/vietnamese.png" width="20"> Vietnamese&nbsp;·&nbsp;<img src="graphics/flags/greek.png" width="20"> Greek&nbsp;·&nbsp;<img src="graphics/flags/georgian.png" width="20"> Georgian&nbsp;·&nbsp;<img src="graphics/flags/divehi.png" width="20"> Dhivehi&nbsp;·&nbsp;<img src="graphics/flags/spanish.png" width="20"> Spanish&nbsp;·&nbsp;<img src="graphics/flags/italian.png" width="20"> Italian&nbsp;·&nbsp;<img src="graphics/flags/german.png" width="20"> German&nbsp;·&nbsp;<img src="graphics/flags/dutch.png" width="20"> Dutch&nbsp;·&nbsp;<img src="graphics/flags/polish.png" width="20"> Polish&nbsp;·&nbsp;<img src="graphics/flags/portuguese-brazil.png" width="20"> Portuguese (Brazil)&nbsp;·&nbsp;<img src="graphics/flags/portuguese-portugal.png" width="20"> Portuguese (Portugal)&nbsp;·&nbsp;<img src="graphics/flags/romanian.png" width="20"> Romanian&nbsp;·&nbsp;<img src="graphics/flags/russian.png" width="20"> Russian&nbsp;·&nbsp;<img src="graphics/flags/slovak.png" width="20"> Slovak&nbsp;·&nbsp;<img src="graphics/flags/turkish.png" width="20"> Turkish&nbsp;·&nbsp;<img src="graphics/flags/hungarian.png" width="20"> Hungarian&nbsp;·&nbsp;<img src="graphics/flags/ukrainian.png" width="20"> Ukrainian&nbsp;·&nbsp;<img src="graphics/flags/finnish.png" width="20"> Finnish&nbsp;·&nbsp;<img src="graphics/flags/french.png" width="20"> French&nbsp;·&nbsp;<img src="graphics/flags/croatian.png" width="20"> Croatian&nbsp;·&nbsp;<img src="graphics/flags/catalan.png" width="20"> Catalan&nbsp;·&nbsp;<img src="graphics/flags/chinese.png" width="20"> Chinese&nbsp;·&nbsp;<img src="graphics/flags/korean.png" width="20"> Korean&nbsp;·&nbsp;<img src="graphics/flags/czech.png" width="20"> Czech&nbsp;·&nbsp;<img src="graphics/flags/swedish.png" width="20"> Swedish&nbsp;·&nbsp;<img src="graphics/flags/japanese.png" width="20"> Japanese&nbsp;·&nbsp;
</details>
- a language selection screen on first launch, plus the system language picker on Android 13+, including regional language variants
<details>... Screenshot of the language selection screen ...</details>
- a complete&nbsp;<img src="graphics/flags/ukrainian.png" alt="UA" width="20">&nbsp;Ukrainian translation (~950 strings), including this README

## Backups in LLX - Narn

- create and restore backups (the TrianguloY fork could only restore)
- archives are now stored in `Documents/Backup/LightningLauncher`, with automatic pickup of backups from previous Lightning Launcher builds

## Google Services

- no dependency on Google Play Services. The only optional piece is the unread Gmail counter. Without Google, everything works fine, you just won't see that number

## UI and UX

### Menus and Settings

- bubble menus:
    - are now dynamic, so you can drag them around the screen. This comes in handy for owners of big-screen phones, tablets, and Android TVs
    - got a "Back" button in nested menus (no need to close and reopen the menu to climb out of deep submenus)
    - have an ID block (the number and code of a desktop element, which you can copy to the clipboard with one tap)
- removed dead links (Google+, "Rate on Play Store") and outdated strings
- every **LLX** - **Narn** settings page now has a "Back" button (no more reaching down to the navigation bar to tap "Back")

---

# Screenshots

<details>... Real shots from a Samsung Galaxy Z Fold8 Ultra will go here ...</details>

---

# Status

- `developer` branch. Started from version 14.3 (patch) of [TrianguloY](https://github.com/TrianguloY/LightningLauncher), current build is 14.60 (dev)
- runs stably on the Samsung Galaxy Z Fold8 Ultra (Android 17), but there's no downloadable APK yet
- the first stable release is coming

---

## Contributing

All feedback, suggestions, and bug reports are welcome. Feel free to ask questions, or if you want to add a new feature to **LLX** - **Narn**, or report a bug, reach out to me here on GitHub in [Issues](https://github.com/Dgikar/LLX-Narn/issues) or on 4PDA in the [Lightning Launcher](https://4pda.to/forum/index.php?showtopic=307407) thread.

Translation texts live in [app/llx/core/src/main/res/values-**XX**/strings.xml](https://github.com/Dgikar/LLX-Narn/tree/developer/app/llx/core/src/main/res)

## License

<a href="LICENSE.md"><img src="https://img.shields.io/badge/license-MIT-blue" alt="License"></a> Copyright (c) 2022-2026 Pierre Hebert, TrianguloY, Dgikar.

[Original](https://github.com/pierrehebert/LightningLauncher) by Pierre Hebert. [Fork](https://github.com/TrianguloY/LightningLauncher) by TrianguloY. [LLX - Narn](https://github.com/Dgikar/LLX-Narn) by Dgikar.
