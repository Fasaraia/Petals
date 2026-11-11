 <p align="center">
  <img width="64" height="64" alt="Petals logo" src="https://github.com/user-attachments/assets/c26170a5-c87a-4490-abf8-fe8da966f459" />
</p>

<h1 align="center">Petals Macro</h1>

<p align="center">
  A lightweight Windows macro recorder and player for mouse and keyboard input.
</p>

---

## Features

- **Record and replay** mouse and keyboard input, including keyboard keys, all three mouse buttons, scrolling, and multi-monitor mouse movement.
- **Adjustable playback speed** to make a macro run faster or slower.
- **Loop playback** a set number of times or indefinitely, with an optional delay between loops.
- **Playback countdown** so you can switch to the target window before a macro starts.
- **Pause and resume** playback using a hotkey.
- **Custom global hotkeys** for recording, playback, and pausing, including modifier combinations such as `Ctrl+Alt+F5`.
- **Live playback status** showing elapsed time, total macro duration, loop progress, and paused state.
- **Macro library** with search, favourites, renaming, and permanent deletion.
- **Reusable playback profiles** for saving different speed, loop, delay, and countdown configurations.
- **Dashboard statistics** for saved macros, completed recordings, playback sessions, and total recording time.
- **Automatic update checks** against the GitHub Releases page.
- Animated menus and custom Petals windows.

## Limitations

- Windows only.
- `Win` / Meta-key hotkeys (for example, `Win+R`) are not currently supported.
- To interact with elevated applications or games, Petals may need to be run as administrator.
- Windows may block input into an elevated application when Petals is not running with the same or higher privileges.

## Installation

1. Download the latest version from [GitHub Releases](https://github.com/Fasaraia/Petals/releases).
2. Run Petals.
3. Open **Settings** to configure playback options and hotkeys.

## Usage

### Default hotkeys

| Action | Default |
|---|---|
| Start / stop recording | `F1` |
| Start / stop playback | `F2` |
| Pause / resume playback | `F3` |

To change a hotkey, open **Settings → Hotkeys**, click the relevant hotkey field, and press the key or key combination you want. Press `Esc` to cancel the selection. The three hotkeys must be different.

> **Tip:** A single key such as `A` will trigger whenever that key is pressed, including while typing. Modifier combinations such as `Ctrl+Alt+R` are less likely to interfere with normal typing.

### Recording a macro

1. Press **Record** or use the recording hotkey.
2. Perform the mouse and keyboard actions you want to capture.
3. Press **Record** again to stop.
4. Use **Save** to name and save the macro.

### Playing a macro

1. Select a macro from **Load**.
2. Adjust playback speed, loops, loop delay, or countdown in **Settings → Playback**, or select a saved profile in **Settings → Profiles**.
3. Press **Play** or use the playback hotkey.
4. Use the pause hotkey to pause or resume. Press **Play** again to stop playback.

## Main window
<img width="312" height="90" alt="image" src="https://github.com/user-attachments/assets/d949f475-85c4-4dce-b308-8f8abc3ba767" />

The main window contains five buttons:

| Button | Function |
|---|---|
| **Save** | Opens a window to name and save the current macro. |
| **Load** | Opens the searchable macro library. |
| **Record** | Starts or stops recording. |
| **Play** | Starts or stops playback. |
| **Settings** | Opens or closes the settings window. |

The status line below the buttons displays the current state. During playback it shows elapsed time, total duration, and loop progress. The playback progress is shown only while a macro is playing or paused.


## Macro library
<img width="152" height="242" alt="image" src="https://github.com/user-attachments/assets/d04d79d5-0573-4fb5-8e6f-a8e09d08500a" /> 

Click **Load** to open the macro library. It lists valid macros saved in the Petals `Macros` folder, along with valid external macros from your recent file history.

- **Search:** Type part of a macro's name into the search field to filter the list.
- **Favourites:** Add frequently used macros to favourites. Favourites are grouped at the top and remain saved after restarting Petals.
- **Load:** Open a macro for playback.
- **Rename:** Opens a custom Petals window to rename the macro. The new name must be valid and cannot already be in use.
- **Remove macro:** Opens a custom confirmation window, then permanently deletes the selected `.pt` file. This is not the same as removing a shortcut from a recent list.
- **Browse…:** Load a `.pt` macro from another location.
- **Open macros folder:** Open the folder where Petals stores its macros.


<img width="165" height="130" alt="image" src="https://github.com/user-attachments/assets/655a8996-a97e-4b58-9035-1a050e6ede68" /> <img width="266" height="130" alt="image" src="https://github.com/user-attachments/assets/cec12ff6-fe4f-4072-816c-da31dbb8eaab" /> <img width="301.47" height="130" alt="image" src="https://github.com/user-attachments/assets/74974f92-645b-4494-8926-334c60767587" />





## Settings

The Settings window contains four tabs.

### Dashboard

Shows:
- Number of macros currently saved in the Petals macro folder.
- Number of completed recordings.
- Number of playback sessions.
- Total recording time.

Statistics are stored locally on the device. Use **Reset Statistics** to reset the counters; this does not delete macros.

<img width="299" height="339" alt="image" src="https://github.com/user-attachments/assets/2bb7f400-c8dc-4eb9-9a71-14de5f80f281" />

### Playback

| Setting | Description |
|---|---|
| **Macro Speed** | Multiplies the recorded timing. `2.0` plays approximately twice as fast; `0.5` plays approximately half as fast. |
| **Loops** | Number of times to play the macro. `0` means repeat indefinitely until stopped. |
| **Delay Between Loops** | Wait time between repetitions, in seconds. |
| **Countdown** | Wait time before playback begins, giving you time to switch to the target window. |

<img width="298" height="339" alt="image" src="https://github.com/user-attachments/assets/9221724c-50a0-4e6c-853c-71af28f7df83" />

### Hotkeys

Configure the global hotkeys for:
- Record / Stop Recording
- Play / Stop Playing
- Pause / Resume
  
<img width="299" height="288" alt="image" src="https://github.com/user-attachments/assets/74fb9717-d93b-40f7-bda8-eccad4545c1a" />

### Profiles

Profiles let you save reusable playback configurations. Each profile can store:
- Playback speed
- Loop count
- Delay between loops
- Countdown

Choose a profile from the dropdown to load its values. Use **Save as New** to create a profile, **Update Selected** to overwrite the selected profile with the current values, and **Delete** to remove it.

Press **Save Settings** to apply the selected profile for playback. Choose **No profile — use Playback settings** to use the values in the Playback tab instead.

<img width="298" height="447" alt="image" src="https://github.com/user-attachments/assets/7e969416-48d1-45b5-8300-a577357d024b" />

## Update checker

Petals checks the latest release on GitHub shortly after startup. If a newer version is available, it displays a notification with a link to the Releases page.

- Update checks run in the background.
- Connection or GitHub API errors are ignored so they do not interrupt recording or playback.
- Petals does not automatically download or install updates.

You can always check manually at [GitHub Releases](https://github.com/Fasaraia/Petals/releases).

## Where files are stored

Petals stores its data in a `Petals` folder:

```text
Petals/
├── macro_settings.json
├── macro_profiles.json
├── petals_stats.json
└── Macros/
    └── YourMacro.pt
```

Petals first tries to use:

```text
C:\Program Files\Petals
```

If that location is not writable, it uses the Windows **Documents** folder instead:

```text
Documents\Petals
```

Use **Load → Open macros folder** to open the actual folder being used on your computer.

- `macro_settings.json` stores application settings, hotkeys, recent macro paths, and favourites.
- `macro_profiles.json` stores playback profiles.
- `petals_stats.json` stores dashboard statistics.
- `Macros/` contains macros saved by Petals.

## Compatibility and notes

- Petals is designed for Windows.
- Run Petals as administrator if you need to record or replay input in an application that is itself running as administrator.
- Keep Petals running while a macro is playing.
- Macros created with older v1.x versions are not compatible with v2.0 and newer because the macro file format changed.

## Support and updates

- **Releases:** https://github.com/Fasaraia/Petals/releases
