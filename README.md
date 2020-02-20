<p align="center">
  <img src="assets/logo.png" alt="Lilly the leoger" />
</p>

[![REUSE status](https://api.reuse.software/badge/github.com/Pext/Pext)](https://api.reuse.software/info/github.com/Pext/Pext)
[![Linux & macOS Build Status](https://travis-ci.org/Pext/Pext.svg?branch=master)](https://travis-ci.org/Pext/Pext)
[![Windows Build status](https://ci.appveyor.com/api/projects/status/73oaa4x1spa5vumx/branch/master?svg=true)](https://ci.appveyor.com/project/TheLastProject/pext/branch/master)
[![ReadTheDocs](https://readthedocs.org/projects/pext/badge/?version=latest)](https://pext.readthedocs.io/en/latest/?badge=latest)
[![Translation status](https://hosted.weblate.org/widgets/pext/-/svg-badge.svg)](https://hosted.weblate.org/projects/pext/)

## Contents

<a href="https://repology.org/metapackage/pext/versions">
  <img align="right" src="https://repology.org/badge/vertical-allrepos/pext.svg?minversion=0.28" alt="Packaging status" />
</a>

- [Introduction](#introduction)
- [How it works](#how-it-works)
- [Installation](https://pext.readthedocs.io/en/latest/installation.html)
- [Usage](#usage)
- [Hotkeys](#hotkeys)
- [Community](#community)
- [License](#license)


## Introduction

Pext stands for **P**ython-based **ex**tendable **t**ool. It is built using Python 3 and Qt5 QML and has its behaviour decided by modules. Pext provides a simple window with a search bar, allowing modules to define what data is shown and how it is manipulated.

For example, say you want to use Pext as a password manager. You load in the pass module, and it will show you a list of your passwords which you can filter with the search bar. When you select a password in the list, it will copy the password to your clipboard and Pext will hide itself, waiting for you to ask for it again.

Depending on the module you choose, what entries are shown and what happens when you select an entry changes. So choose the module appropriate for what you want to do, and Pext makes it easy.

Several modules are available for effortless install right within Pext.

![Pext Introduction](/assets/pext_intro.gif)

## How it works

Pext is designed to quickly pop up and get out of your way as soon as you're done with something. It is recommended to bind Pext to some global hotkey, or possibly run multiple instances of it with different profiles under multiple hotkeys. Example Pext workflows look as follows:

![Pext workflow graph](/assets/workflow_graph.png)

Simply put:

- Open (Pext)
- Search (for something)
- Select (with Enter)
- Hide (automatically)

## Usage

To actually use Pext, you will first have to install one or more modules. Check out the Pext organisation on [GitHub](https://github.com/Pext) or use `Module` -> `Install module` -> `From online module list` in the application for a list of modules.

After installating at least one module, you can load it from the `Module` -> `Load module` menu. After that, experiment! Each module is different.

For command line options, use `--help`.

### Hotkeys

**Entry management:**
- Escape: Go one level up
- Tab: Tab-complete the current input
- Enter / Left mouse button: Select entry or run command
- Shift+Enter: Select entry or run command but explicitly disable minimizing
- Ctrl+Enter: Run command with arguments
- Ctrl+. / Right mouse button on any item: Open context menu
- Ctrl+J / Down arrow: Go one entry down
- Ctrl+H / Up arrow: Go one entry up
- Ctrl+F / Page down: Go one page down
- Ctrl+B / Page up: Go one page up

**Tab management:**
- Ctrl+T: Open new tab
- Ctrl+W: Close current tab
- Ctrl+Tab: Switch to next tab
- Ctrl+Shift+Tab: Switch to previous tab
- Alt+`<number>`: Switch to tab `<number>`
- F5: Reload tab, including code changes to the module

**Session management:**
- Ctrl+Q: Quit

## Community

<a href="https://hosted.weblate.org/engage/pext/?utm_source=widget"><img src="https://hosted.weblate.org/widgets/pext/-/multi-auto.svg" alt="Translation status, hosted by Weblate" align="right" /></a>

If you need support or would like to join our user community, you have several options:

[![Matrix](https://img.shields.io/matrix/pext:matrix.org.svg?color=royalblue&label=Matrix%20Channel&logo=matrix&style=for-the-badge)](https://riot.im/app/#/room/#pext:matrix.org)
![Telegram Join Group](https://img.shields.io/static/v1?link=https://t.me/PextTool&link=https://web.telegram.org/%23/im%3Fp%3D%40PextTool&label=Telegram%20Group&message=Join%20Us&style=for-the-badge&logo=telegram&labelColor=darkslategrey&color=royalblue)
![IRC Channel](https://img.shields.io/static/v1?link=ircs://irc.freenode.net:6697/%23pext&link=https://webchat.freenode.net/%3Fchannels=%23pext&label=Freenode%20IRC&message=Webchat&style=for-the-badge&labelColor=darkslategrey&color=royalblue&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABQAAAAUCAMAAAC6V+0/AAABpFBMVEUAAAABr+8Br+8Br+8Ar+8Br+8Ar+8Ar+8Ar+8Ar+8Ar+8Ar+8Ar+8Ar+8Ar+8Ar+8Ar+8Ar+8Ar+8Ar+8Ar+8Ar+8Ar+8Ar+8Ar+8Ar+8Ar+8Ar+8Ar+8Ar+8Ar+8Ar+8Ar+8Ar+8Ar+8Ar+8Ar+8Ar+8Ar+8Ar+8Ar+8Ar+9HtfAAr+8Ar+8Ar+8Ar+8IsO8Wse8Ar+9UufELsO8Ar+97xPMAr+8Ar+8Ar++PyvQAr+9cu/GMyvQAr+8Ar+8Ar+9AtvCYzfQ/tfCGyPMAr+8CsO8Dr+8MsO8bse9DtvBOt/BRuPBXu/FauvFhvPFuwPJ7wvJ8w/J9xPOFx/OSy/SSzPSXzvSZzvSZz/Wf0fWi0vWk0vWl0vWn0/Wp1PWq1Pav1/aw2Paw2fe02ve22/e42/e73fe83fe/3ve/3/jB4PjC4fjE4fjG4vjH5PnL4/nM5PnN5fnO5vnR5vnU6PrV6vrf7vvk8fzn8vzo8/zp8/zq9Pzr9Pzs9Pzs9f3s9v3v9/3v+P3w9/30+v72+/74/P76/P76/f77/f79/v/+//////+f7KdqAAAARHRSTlMACQoLFBUWHzM0NTY7PkRNWlteYmNlZmdqcXJzfn+DhoeIiZCRlpeYmZqgo6Slpq6xtLzAyc3f4eTm5+fn6PP09PT7/GttYioAAAETSURBVBgZXcEHNwJgGAbQ16zIlpW9ishW9nrsvWdlb5KZvaOeP+3jHEe5V35kVZuKEiVcGy1BasnHvuyEBZejJUV+NZEPQOE1OdMeK0p5Q5VplTwH6gLkKJJFaSUDH+TdvmuHfAMKtCLiZIjXLbtGIpYY6gSlEmnDwBzp33Sf+vhtA2YRfQfmSS+AJ3J6ZHII+RKXmWHdJj1AN8lBKAYxnF157snjifEe8gUoMabFSfEz/3xeuPc79SJm/tNvi5LKqZVd0ue99fNHAAgTjR0O8hLAO7nuWtsDRERXeEQeAmNkoBdKsyjpB96nZVR0kTeA2VJvESWmHUre8KJzFm3yK7URQHwOlBoJpouQpNwyq1G+fQEQZXehhn461QAAAABJRU5ErkJggg==)

All of these channels are linked to each other, so there is no need to worry about missing out. You can also follow our project announcements on Twitter.

![Twitter Follow](https://img.shields.io/twitter/follow/PextTool?link=https://twitter.com/PextTool&color=royalblue&logo=twitter&logoColor=lightskyblue&style=for-the-badge)

The chart at right shows our progress in making Pext a tool for anyone who wants it, regardless of what language they speak. If you are fluent in one of the languages with a translation in progress or one that we have yet to add to the list, clicking the chart will take you to our [project page at Weblate](https://hosted.weblate.org/projects/pext/) where you can register for a free account and be busy translating within minutes, wrapped in the embrace of our most sincere gratitude.

## Licensing

### Source code: <img src="https://img.shields.io/static/v1?link=https://spdx.org/licenses/GPL-3.0-or-later.html&link=https://github.com/Pext/Pext/blob/master/LICENSES/GPL-3.0-or-later.txt&logo=spdx&label=SPDX%20License%20Identifier&message=GPL-3.0-or-later&labelColor=darkslategrey&color=a3312f&style=for-the-badge" alt="SPDX GPL-3.0-or-later" align="right">

<br clear="right"/>

The Pext source code is licensed under the [GNU General Public License 3.0](LICENSES/GPL-3.0-or-later.txt).

### Documentation/artwork: <img src="https://img.shields.io/static/v1?link=https://spdx.org/licenses/CC-BY-SA-4.0.html&link=https://github.com/Pext/Pext/blob/master/LICENSES/CC-BY-SA-4.0.txt&logo=spdx&label=SPDX%20License%20Identifier&message=CC-BY-SA-4.0&labelColor=darkslategrey&color=ef653a&style=for-the-badge" alt="SPDX CC-BY-SA-4.0" align="right">

<br clear="right"/>

The artwork and documentation that accompany Pext (filenames specified below) are licensed under the [Creative Commons Attribution Share-Alike License 4.0](LICENSES/CC-BY-SA-4.0.txt).
- assets/
- docs/
- pext/images/
- .github/
- All files in the repository root ending in ".md"

#### Logo

<a href="https://www.whitepaperfox.com/"><img src="https://user-images.githubusercontent.com/15098724/74970294-f5c83e00-53d2-11ea-9792-272978caeec2.png" alt="Pext logo / Lilly the Leoger by White Paper Fox" align="right" height="92px"></a>
The Pext logo (seen at right, graciously provided by [**vaeringjar**](https://notabug.org/vaeringjar)), if used elsewhere, should be attributed as _"Lilly the leoger"_ by White Paper Fox, or simply as _"Pext logo"_ (at your option). Please link the image to Pext (at <https://github.com/Pext/Pext> or <https://pext.io/>) and to White Paper Fox (at <https://www.whitepaperfox.com/>) where possible.
