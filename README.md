# RemindersMenubar

A lightweight macOS application that displays your Apple Reminders directly in your Mac's menu bar. 

## Features

* **Quick Access**: View your active to-do items instantly from any screen.
* **Native Integration**: Seamlessly syncs and fetches live data directly from the native Apple Reminders app.

## Requirements

* **Operating System**: macOS 11.0 (Big Sur) or later.

## Installation

1. Download the latest release from the [Releases](https://github.com) page.
2. Unzip the downloaded file.
3. Drag **RemindersMenubar.app** into your **Applications** folder.
4. Launch the app from your Applications folder or Launchpad.

## Prerequisites & Permissions

Because this application reads data from your native ecosystem, you must grant it permission to access your reminders.

1. Open **System Settings** on your Mac.
2. Navigate to **Privacy & Security** > **Reminders**.
3. Toggle the switch next to **RemindersMenubar** to **Allow**.

## Building From Source

If you prefer to compile the application yourself using Xcode:

1. Clone the repository:
   ```bash
   git clone https://github.com
   ```
2. Open `RemindersMenubar.xcodeproj` in Xcode.
3. Select your target device (Mac) and build scheme.
4. Go to **Product** > **Archive** or **Build** to generate the app binary.

## Troubleshooting

If you encounter any security or signature errors when launching the application, you can manually sign the app binary using the macOS Terminal.

Run the following command:

```bash
codesign --force --deep --sign - /path/to/remindersmenubar.app
```

> **Tip**: Instead of typing out the full path, type `codesign --force --deep --sign - ` and then drag and drop the application icon directly from Finder into your Terminal window to automatically insert the correct path.

## Contributing

Contributions are welcome! If you would like to help improve this project:

1. Fork the repository.
2. Create a new branch for your feature or bug fix: `git checkout -b feature-name`.
3. Commit your changes with descriptive messages.
4. Push your branch to GitHub: `git push origin feature-name`.
5. Open a **Pull Request** detailing your changes.

For major modifications, please open an issue first to discuss what you would like to change.

## License

This project is licensed under the **GNU General Public License v3.0** — see the [LICENSE](https://github.com) file for details.
