# <img width="64" height="64" alt="logo" src="https://github.com/user-attachments/assets/c26170a5-c87a-4490-abf8-fe8da966f459" /> Petals Macro

Just your regular input detector and replay macro

## Features

* Record and replay mouse + keyboard input (all keys, all three mouse buttons, scroll, multi-monitor)
* Custom playback speed
* Loop count (or infinite replay) with a delay between loops
* Countdown before playback so you can switch windows
* Pause / Resume while a macro is playing
* Pick **any** hotkey, including combos with `Ctrl`, `Alt` and `Shift` (e.g. `Ctrl+Alt+F5`)
* Live status line: recording timer, macro length, loop counter, paused state
* Save & Load macros, with a recent files list (add / remove / clear)
* Smooth animations on startup, shutdown and menus

## Not Features (Things I'm too stupid/lazy to figure out)

`Win` / Meta key hotkeys (e.g. `WIN+R`) <---- Lazy

Closing keybind (Right-click the bar → **Exit**, or close it from the taskbar) <---- Lazy

## To Be Added

Mpos accuracy option - Let users pick Mouse Position accuracy in exchange for larger file size

<sub> (Potentially causes replay delay due to high amount of inputs) </sub>

## Usage

Keybinds by default are:

| Action | Default |
| ------ | ------- |
| ``Record / Stop Recording`` | ```F1``` |
| ``Play / Stop Playing`` | ```F2``` |
| ``Pause / Resume`` | ```F3``` |

Click a hotkey box in Settings and press the key or combo you want. `Esc` cancels. The three hotkeys must all be different.

> Tip: a hotkey with no modifier (like `A`) fires every time you type that key. Combos like `Ctrl+Alt+R` avoid that.

## Main UI

Button Usages in Order:

|| ``Save`` | ``Load`` | ``Record`` | ``Play`` | ``Settings`` ||

<img width="321" height="87" alt="Screenshot 2025-10-18 101642" src="https://github.com/user-attachments/assets/0326545c-2a86-40b8-a309-a053f7dd04ed" />

The line under the buttons shows what Petals is doing: `Recording 0:05.3`, `Ready · 0:12.0`, `Playing 2/10 · F3 to pause`, `Paused`, and so on.

| Button | What it does |
|--------|--------------|
| **Save** | Asks for a name and saves the macro into the `Macros` folder. Naming an existing macro asks before replacing it. |
| **Load** | Opens your recent macros. Click one to load it. |
| **Record** | Starts / stops recording. |
| **Play** | Starts / stops playback. |
| **Settings** | Opens the settings window. |

Right-click the bar for **Exit**.

### Load menu

| Item | Description |
|------|-------------|
| Recent macros | The last 20 macros you saved or loaded. Greyed out if the file no longer exists. |
| **Browse…** | Pick a `.pt` file from disk. |
| **Add files…** | Add one or more `.pt` files to the list without loading them. |
| **Open macros folder** | Opens the folder where macros are saved. |
| **Remove** | Removes an entry from the list (the file itself is never deleted). |
| **Clear list** | Empties the list. |

## Settings

<img width="233" height="381" alt="Screenshot 2025-10-18 101706" src="https://github.com/user-attachments/assets/518e3014-8ce0-445c-94fb-d1ffc336ebdf" />

### Settings Breakdown

| Setting                     | Description |
|--------------------------|------------|
| **Macro Speed**           | Multiplies the original macro timing. Example: `2.0` makes the macro replay twice as fast, `0.5` makes it slower. |
| **Loops**                 | How many times the macro plays. `0` means infinite, and it loops until you stop it. |
| **Delay Between Loops (s)** | Waits this long between loops. Useful for macros that need cooldown or reset time. |
| **Countdown (s)**         | Counts down before playback starts (0 to 60 seconds) so you have time to switch windows. |
| **Hotkeys**               | Record, Play and Pause keys. Hotkeys are global, so they work even when the app is not focused. |

Press **Save** to apply and store your settings. They are restored next time you launch the app.

## Where files are stored

Petals keeps everything in one folder:

```
Petals\
  macro_settings.json
  Macros\
    your macros.pt
```

* If Petals can write to it, the folder is `C:\Program Files\Petals` (this needs the app to run as administrator).
* Otherwise it uses `Documents\Petals`.

Use **Load → Open macros folder** to see exactly where it is.

## Notes

* Windows only.
* To record or replay into elevated (administrator) windows or games, run Petals as administrator. Windows blocks it otherwise.
* Macros from v1.x (`.pt` files) are **not compatible** with v2.0 and newer. The file format changed so every key can be recorded.
