# PackTracker [![Github All Downloads](https://img.shields.io/github/downloads/mgk82/packtracker/total.svg)](https://github.com/mgk82/packtracker/releases)
Plugin for [HearthstoneDeckTracker](https://hsdecktracker.net/)

> **This fork** ([mpcaren/PackTracker](https://github.com/mpcaren/PackTracker)) updates the plugin for current
> Hearthstone Deck Tracker versions (1.53.x). Changes from [the original](https://github.com/MGK82/PackTracker):
> - Fixed plugin loading against current HDT (removed/renamed APIs)
> - Fixed the Forged in the Barrens booster id (packs were shown as a number)
> - Added pack names for all sets through Showdown in the Badlands
> - Packs from sets newer than the bundled data are now named automatically
>   from their card contents, so future expansions display correctly without updates
>
> ### Building
> Requires the .NET SDK and an installed copy of Hearthstone Deck Tracker (the build
> references HDT's assemblies from your local install — newest `app-*` folder is
> auto-detected, override with `-p:HDTPath=<folder>`):
> ```
> dotnet build PackHistorian\PackTracker.csproj -c Release
> ```
> Then copy `PackHistorian\bin\Release\net481\PackTracker.dll` to
> `%AppData%\HearthstoneDeckTracker\Plugins\` and restart HDT.

Pack Tacker is a small but handy plugin for Hearthstone Deck Tacker that allows you to keep an eye on every pack you open. 
This allows you to see how many cards of different rarities have dropped over time and also enables you to estimate when your next Epic or Legendary is coming!

## Features [![GitHub Latest](https://img.shields.io/github/release/mgk82/packtracker.svg)](https://github.com/MGK82/PackTracker/releases/latest) [![Github Latest Downloads](https://img.shields.io/github/downloads/mgk82/packtracker/latest/total.svg)](https://github.com/MGK82/PackTracker/releases/latest)
- Tracks your pack openings
  - **Fully Automatic. No hassle with spreadsheets or any other manual input**
- Data can be represented in
  - a date-based (calender-like) history
  - a boosterpack-series-based statistic
  - a plain chronological text-log
- Supports auto-update
- Counts boosterpack-series-based **Pity Timer** for Epic and Legendary cards
  - Represented as bar charts
  - Overlay while opening packs (See your pity timers counting live)
- Can search through card names and texts in both, english and the chosen language of your HDT at once
  - *HDT must support the translation*
- **All stored locally. No hassle with overloaded webpages on release days**

[Download](https://github.com/MGK82/PackTracker/releases/latest)  and unzip  
[How to add plugins to HDT](https://github.com/HearthSim/Hearthstone-Deck-Tracker/wiki/Available-Plugins)

## Screenshots

Pity Timers  
![](https://github.com/MGK82/PackTracker/blob/master/doc/Screenshots/PityTimer.png?raw=true)

Statistic  
![](https://github.com/MGK82/PackTracker/blob/master/doc/Screenshots/Statistic.png?raw=true)

History  
![](https://github.com/MGK82/PackTracker/blob/master/doc/Screenshots/History.png?raw=true)  

Log  
![](https://github.com/MGK82/PackTracker/blob/master/doc/Screenshots/Log.png?raw=true)

Search  
![](https://github.com/MGK82/PackTracker/blob/master/doc/Screenshots/Search.png?raw=true)
