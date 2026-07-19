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
