


[README.md](https://github.com/user-attachments/files/30163384/README.md)
<div align="center">
  <img
    src="docs/images/reminders-icon.png"
    alt="Reminders MenuBar"
  >
  <h1>
    Reminders MenuBar
  </h1>
  <p>
    Simple macOS menu bar app to view and interact with reminders.
  </p>
  <p>
    <a href="#features">Features</a> •
    <a href="#installation">Installation</a> •
    <a href="#permission-request">Permission Request</a> •
    <a href="#contributing">Contributing</a> •
    <a href="#languages">Languages</a> •
    <a href="#license">License</a>
  </p>
</div>

<div align="center">
  <img
    max-width="400"
    width="45%"
    src="docs/images/reminder-menubar-light.png"
    alt="Reminders MenuBar in light mode"
  >
  <img
    max-width="400"
    width="45%"
    src="docs/images/reminder-menubar-dark.png"
    alt="Reminders MenuBar in dark mode"
  >
</div>

## Features

* All interactions through the macOS menu bar
* Keep everything in sync with Apple Reminders
* Create new reminders using natural language for due dates, lists, and tags
* Mark as completed or edit due dates, priorities, recurrences, lists, tags, and more
* View upcoming reminders with a configurable time interval
* Search across all your reminders
* Filter reminders through lists and tags
* Customize the menu bar with icon, counter, or next upcoming reminder
* Toggle the app with a global keyboard shortcut

<div align="center">
  <img
    src="docs/images/reminders-menubar-demo.gif"
    alt="Reminders MenuBar demo"
  >
</div>

## Installation

*Reminders MenuBar requires macOS Big Sur 11 or later.*

### Homebrew

Reminders MenuBar can be installed using [Homebrew](https://brew.sh).

```bash
brew install --cask reminders-menubar
```

### Direct Download

Direct downloads are available on the [releases page](https://github.com/DamascenoRafael/reminders-menubar/releases):

* Disk image (`.dmg`): double-click to open, then drag the app to *Applications*
* Zip archive (`.zip`): extract and drag the app to *Applications*

## Permission Request

Reminders MenuBar uses [EKEventStore](https://developer.apple.com/documentation/eventkit/ekeventstore) to access reminders on macOS (which are available in Apple Reminders and can be synced through iCloud). On first use, the app should request permission to access reminders as shown in the image below. Also, in *System Settings > Privacy & Security > Reminders* it is possible to manage this permission. [Click here if you are using *OpenCore Legacy Patcher*](docs/fix-for-opencore-legacy-patcher.md).

<div>
  <img
    width="250"
    src="docs/images/reminders-permission.png"
    alt="macOS window asking permission for Reminders MenuBar to access reminders"
  >
</div>

## Contributing

Feel free to share, open issues and contribute to this project! :heart:

## Languages

🇺🇸 English • 🇧🇷 Brazilian Portuguese • 🇨🇳 Chinese (Simplified and Traditional) • 🇨🇿 Czech • 🇳🇱 Dutch • 🇵🇭 Filipino • 🇫🇷 French • 🇩🇪 German • 🇮🇩 Indonesian • 🇮🇹 Italian • 🇯🇵 Japanese • 🇰🇷 Korean • 🇵🇱 Polish • 🇷🇺 Russian • 🇸🇰 Slovak • 🇲🇽 Spanish (Latin America) • 🇹🇷 Turkish • 🇺🇦 Ukrainian • 🇻🇳 Vietnamese

[▶︎ Click here to learn how to add new languages :globe_with_meridians:](docs/adding-new-languages.md)

## License

This project is licensed under the terms of the GNU General Public License v3.0.  
See [LICENSE](LICENSE) for details.

[README.md](https://github.com/user-attachments/files/30163382/README.md)
# RemindersMenubar

A lightweight macOS application that displays your Apple Reminders directly in your Mac's menu bar. 

## Features

* **Quick Access**: View your active to-do items instantly from any screen.
* **Native Integration**: Seamlessly syncs and fetches live data directly from the native Apple Reminders app.

## Requirements

* **Operating System**: macOS 14.0 (Sonoma) or later. Should work on macOS 26 and 27 beta ( developer beta 5, public beta 1).

## Installation

1. Download the latest release from the [Releases](https://github.com/TheShadowNinjaGMD/remindersmenubar/releases) page.
2. Unzip the downloaded file or drag it into your Applications folder if using the dmg file.
3. Drag **RemindersMenubar.app** into your **Applications** folder.
4. Launch the app from your Applications folder or Launchpad.

## Prerequisites & Permissions

Because this application reads data from your native ecosystem, you must grant it permission to access your reminders.
Clicking it may open a pop-up window asking for permission ignore the below if it appears and just click allow.

1. Open **System Settings** on your Mac.
2. Navigate to **Privacy & Security** > **Reminders**.
3. Toggle the switch next to **RemindersMenubar** to **Allow**.

## Building From Source
# Do this if you want to contribute to the project and want to build the application yourself with any edits you want.
If you prefer to compile the application yourself using Xcode:

1. Clone the repository:
   ```bash
   git clone https://github.com/TheShadowNinjaGMD/remindersmenubar/
   ```
2. Open `RemindersMenubar.xcodeproj` in Xcode.
3. Select your target device (Mac) and build scheme.
4. Go to **Product** > **Archive** or **Build** to generate the app binary.

## Troubleshooting

If you encounter any security or signature errors when launching the application, you can manually sign the app binary using the macOS Terminal.

Run the following command:

```bash
codesign --force --deep --sign - /Applications/Reminders\ MenuBar.app
```

> **Tip**: Instead of typing out the full path, type `codesign --force --deep --sign - ` and then drag and drop the application icon directly from Finder into your Terminal window to automatically insert the correct path.

## Contributing

Contributions are always welcome! Please read our [Contributing Guidelines](CONTRIBUTING.md) to learn about our development workflow, reporting bugs, and submitting pull requests. For major modifications, please open an issue first to discuss what you would like to change.

## License

This project is licensed under the **GNU General Public License v3.0** — see the [LICENSE](https://github.com/TheShadowNinjaGMD/remindersmenubar/blob/main/LICENSE) file for details.
