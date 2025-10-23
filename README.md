# <img width="64" height="64" alt="logo" src="https://github.com/user-attachments/assets/c26170a5-c87a-4490-abf8-fe8da966f459" /> Petals Macro

Just your regular input detector and replay macro

## Features

* Custom Playback Speed
* Infinite Replay
* Add Extra End delay
* Save & Load Files
* Combo Keys (anything like CTRL+SHIFT+5)

## Not Features (Things I'm too stupid/lazy to figure out)

Alt Combo Key, Meta Key Ect Inputs (Aka ALT+T, WIN+R ect) <---- Lazy

Closing Keybind (Just close it from the taskbar) <---- Lazy

## To Be Added

Mpos accuracy option - Let users pick Mouse Position accuracy in exchange for larger file size 

<sub> (Potenially causes replay delay due to high amount of inputs) </sub>

Timer - I uh...


## Usage

Keybinds by default are:

``Record/Stop Recording`` : ```F1```

``Play / Pause`` : ```F2```

<details>

<summary>All Keybinds Available in Settings</summary>

| Key        | Description                        |
| ---------- | ---------------------------------- |
| `F1`       | Global (can be used for both)      |
| `F2`       | Global                             |
| `F7`       | Global                             |
| `F8`       | Global                             |
| `SHIFT+F1` | Global                             |
| `SHIFT+F2` | Global                             |
| `SHIFT+F7` | Global                             |
| `SHIFT+F8` | Global                             |
| `SHIFT+P`  | Exclusive (Play / Stop Play Only   |
| `SHIFT+R`  | Exclusive (Record / Stop Recording |

</details>

## Main UI

Button Usages in Order: 

|| ``Save`` | ``Load`` | ``Record`` | ``Play`` | ``Settings`` ||

<img width="321" height="87" alt="Screenshot 2025-10-18 101642" src="https://github.com/user-attachments/assets/0326545c-2a86-40b8-a309-a053f7dd04ed" />

## Settings

<img width="233" height="381" alt="Screenshot 2025-10-18 101706" src="https://github.com/user-attachments/assets/518e3014-8ce0-445c-94fb-d1ffc336ebdf" />

### Settings Breakdown

| Setting                     | Description |
|--------------------------|------------|
| **Playback Speed**        | Multiplies the original macro timing speed. Example: `2.0` makes the macro replay twice as fast, `0.5` makes it slower. |
| **Extra End Delay (S)**  | Adds a final delay after all events have finished before looping or ending. Useful for macros that require cooldown or reset time. |
| **Infinite Loop** | Choose how many times the macro should replay. When **Infinite Replay** is enabled, replay loops endlessly until manually stopped. |
| **Global Hotkeys**        | Customize the hotkeys for Recording, and Playback. Hotkeys are registered globally, meaning they work even when the app is not focused. |
| **Save Settings on Exit** | Automatically saves your chosen settings and hotkeys so they're restored next time you launch the app. |
