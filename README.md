**This is a fork of AndreAle94's MoneyWallet app: [Original source code](https://github.com/AndreAle94/moneywallet).**

I created this because original app isn't fully FOSS, and because development process is too slow.

I want to create a better app with more modern UI, and without any non-free libraries.

# MoneyWalletX - Expense Manager
[![License](https://img.shields.io/badge/license-GPL%20V3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0.html)
MoneyWallet is an application designed to help you keep track of your expenses. This repository contains the source code of the latest version, completely rewritten from scratch.

### Redistributing this app as your own is NOT permitted.

# Table of Contents

1. [History](#history)
2. [Donations](#donations)
3. [Build](#build)
4. [FAQ](#faq)
5. [Credits](#credits)
6. [License](#license)

## History
I have been working behind this project for a long time, originally born as a tool to learn Android development, it has evolved over time and has recently been completely revised as a university project for the DIMA course at Politecnico di Milano.
As you may have noticed, the previous version on the PlayStore required a small in-app purchase to handle more than just one wallet. The idea was to invest the money earned to pay for my studies, unfortunately among the interest rates of the PlayStore and the local taxes of the individual countries the profit was practically derisory. I did not had the opportunity to continue the development with continuity due to the university and the little free time available. Only recently I had the opportunity to get the project in hand and I decided to make it open source. In this way, anyone who wants can contribute.

## Donations
I'm not ready to receive donations, send all to [original app developer](https://github.com/AndreAle94/moneywallet) for now.

## Build
You can compile the application very simply: just clone this repository locally to your computer and Android Studio will take care of the rest.
You have four different options to build it with two choices.
The first choice is which version you want to build:

- proprietary: this build flavor is designed to integrate Google Drive and Dropbox for a better user experience. It contains proprietary libraries (not open source) and requires the inclusion of valid api-keys to use these services. These keys must be registered in the file called gradle.properties in the root folder of the project before compiling.
- floss: this build flavor is designed to contain only open source code and for this reason the integration with Google Drive and Dropbox has been removed.

The second choice is which map provider you want to use and you can choose between:

- gmap: this build flavor uses Google Map as map provider and requires you to provide a valid API-key. This key must be registered in the file called gradle.properties in the root folder of the project before compiling.
- osm: this build flavor uses OpenStreetMap as map provider.

To decide what kind of build to compile, use the appropriate menu of gradle to choose the desired combination of build flavors.
If you want to build only open source code (e.g. for the F-Droid market) you should use 'floss' and 'osm'.

The current release in Google Play Store uses 'proprietary' and 'osm' with some changes to integrate also the Crashlytics framework and the In-App billing library.

## FAQ
1. why does the precompiled binary contain a huge icon pack while there are only a few icons in the source code?
  The icon pack license clearly states that the icons can not be distributed publicly. If you want to have the same package of icons you will have to buy them on their website. The few icons in the repository come from their small free icon pack with a license that allows their free use.
2. Is this project still in development? Currently I do not have much time to devote to the project, as already explained I am a university student close to graduation and very busy. I can work on it from time to time but I can't promise continued and lasting support.
3. Can i contribute to this project? Oh yes! You can freely fork this project and open new pull requests. Translations in other languages are also welcome (you will be credited within the application).

## Credits
- [Adam Lapinski](http://www.yeti-designs.com): author of the awesome logo.
- [Freepik](https://www.freepik.com): source of first-start images.
- [RoundIcons](https://roundicons.com): source of the internal icon-pack.

## License
    Copyright (c) 2018.
    This program is free software: you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation, either version 3 of the License, or
    (at your option) any later version.

    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.

    You should have received a copy of the GNU General Public License
    along with this program.  If not, see <http://www.gnu.org/licenses/>.
