<p align="center">
  <img src="logo.gif" alt="Aktashef" width="140">
</p>

# Aktashef | اكتشف الثقافات

An iOS app that helps Saudi travelers avoid cultural misunderstandings abroad. Pick a destination and get simple, Arabic-first guidance on local customs, what to do, and what to avoid. Everything works offline.

Built as a team challenge at the **Apple Developer Academy**.

![Swift](https://img.shields.io/badge/Swift-F05138?logo=swift&logoColor=white)
![SwiftUI](https://img.shields.io/badge/SwiftUI-0D96F6?logo=swift&logoColor=white)
![iOS](https://img.shields.io/badge/iOS-17+-000000?logo=apple&logoColor=white)

## What it does

- Browse countries as a list or a grid, and search by name.
- Open a country to read its customs, do's and don'ts, grouped by category.
- Save favorite countries for quick access. Favorites are stored on the device.
- Works with no internet: all content ships inside the app as JSON.
- Arabic interface with right-to-left layout, an animated splash screen, and light and dark mode.

## Tech stack

Swift, SwiftUI, SwiftData, JSON for content, `FileManager` for saving favorites.

## Run it

You need Xcode 16+ on a Mac.

```bash
git clone https://github.com/FaiAlharthi/Aktashef.git
cd Aktashef
open CultreApp.xcodeproj
```

Pick an iPhone simulator and press Run.

## How it works

- `countries.json`, `catagory.json`, and `catagoryContent.json` hold the countries, the categories, and the cultural content.
- On first launch the countries file is copied from the app bundle into the Documents folder, so favorites can be saved and survive restarts (`DataLoader.swift`).
- `CountryListView`, `CountryGridView`, and `CountryDetailView` are the three main screens.

## What I would improve next

- Use SwiftData directly for favorites instead of rewriting a JSON file.
- Rename `Counrtry`/`catagory` identifiers to the correct spelling.
- Add more countries and an English interface.

## Team

Built by **Swift Squad**.

<table>
  <tr>
    <td align="center"><a href="https://github.com/FaiAlharthi"><b>Fai Alharthi</b></a></td>
    <td align="center"><a href="https://github.com/Aljoharah25"><b>Aljoharah Bin Taleb</b></a></td>
    <td align="center"><a href="https://github.com/joudy003"><b>Joud Alamri</b></a></td>
    <td align="center"><a href="https://github.com/batoul252"><b>Albatoul Alhamas</b></a></td>
    <td align="center"><a href="https://github.com/ManarAliAlghamdi"><b>Manar Alghamdi</b></a></td>
  </tr>
</table>
