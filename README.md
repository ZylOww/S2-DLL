# S2C WWII Speedrun DLL

This is a speedrun-oriented DLL for Call of Duty: WWII that aims to enhance the speedrunning experience by implementing rebindable restart keys, infinite consumables, and a session-based verification watermark.

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

* **SHA-256**: `0fe68f2bbdc327e119ce4685eb672c2884ff72eec54cc13a8e92a1997855cbaa`
* **VirusTotal**: [View Scan Report](https://www.virustotal.com/gui/file/0fe68f2bbdc327e119ce4685eb672c2884ff72eec54cc13a8e92a1997855cbaa?nocache=1)

## Support & Contact
If you run into any bugs, have suggestions for new features, or need help with setup, feel free to reach out.

* **Discord**: itszylow
* **GitHub**: Open an [Issue](https://github.com/ZylOww/S2-DLL/issues)
