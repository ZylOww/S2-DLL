# S2C WWII Speedrun DLL

This is a speedrun-oriented DLL for Call of Duty: WWII that aims to enhance the speedrunning experience by implementing rebindable restart keys, soft consumables, and a session-based verification watermark.

---

## Core Features
* **Custom Keybinds**: Use the ImGui menu to rebind Fast Restart and Map Restart to any key.
* **Soft Consumables**: Implements a toggle for consumables allowing you to "softly" have 999 (non-permanent) for any consumable you currently own. Note: Consumables with a quantity of 0 will not be granted the infinite quantity.
* **Focus Detection**: Built-in checks ensure the game is the active window before triggering any hotkeys, preventing accidental restarts while tabbed out.
* **ImGui Overlay**: Press **INSERT** to toggle the configuration menu.

## Verification & Anti-Splicing
To ensure runs are legitimate for leaderboards, the DLL draws a small watermark in the top-left corner of the screen:

**Format**: `s2-[Version]-[Static Timestamp]-[Session ID]-[Unix Timestamp]`

The **Session ID** is a randomized string that regenerates every time a Fast Restart or Map Restart is triggered. This confirms the run was completed in one continuous session. The **Unix Timestamp** provides a live clock to verify that the footage has not been edited or manipulated.

## How to use
1. Download `s2_main.dll` from the [Releases](https://github.com/ZylOww/S2-DLL/releases) tab.
2. Inject the DLL into the Call of Duty: WWII process using your preferred injector.
3. Press **INSERT** to open or hide the menu.

## Integrity
This DLL is closed-source. Please use the SHA-256 hash below to verify that your file has not been tampered with. If the file is flagged by your anti-virus, you may need to add an exclusion.

* **SHA-256**: `24B038C01896392EB13226BDF965DAD36F1A03B5E5E6150B93AD5F7497D617E6`
* **VirusTotal**: [View Scan Report](https://www.virustotal.com/gui/file/24b038c01896392eb13226bdf965dad36f1a03b5e5e6150b93ad5f7497d617e6)

## Support & Contact
If you run into any bugs, have suggestions for new features, or need help with setup, feel free to reach out.

* **Discord**: itszylow
* **GitHub**: Open an [Issue](https://github.com/ZylOww/S2-DLL/issues)
