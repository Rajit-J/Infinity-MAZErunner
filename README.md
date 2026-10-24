# Infinity Maze Runner

An arcade maze game with a browser edition and an original Raylib-based C desktop edition.

## Browser edition

- Fresh, open maze layouts with connected walkable space.
- Randomly wandering enemies with wall-aware movement.
- Collectibles, score progression, pause/menu controls, and responsive touch controls.
- Original ambient background audio, enabled after user interaction.

### Run on Windows

The web edition is static and requires no package installation. In PowerShell:

```powershell
cd D:\MyProjects\Infinity-MAZErunner
py -m http.server 5176 --bind 127.0.0.1 --directory web
```

Open [http://127.0.0.1:5176](http://127.0.0.1:5176). Stop the server with **Ctrl+C**.

Use **W/A/S/D** or arrow keys to move; use the on-screen controls on touch devices. Press **P** to pause/resume and **Escape** to return to the menu. Browser audio requires a user gesture.

## Desktop edition

The C desktop game uses Raylib. Run the included executable if it is provided for your platform:

```powershell
.\maze_runner.exe
```

To build from source on Windows, install the Raylib development files at `C:\raylib` as expected by the Makefile, then run the project's documented build command. Close the game window to exit.

## Technology

- Browser edition: HTML, CSS, and JavaScript
- Desktop edition: C and Raylib

## Before publishing

Do not commit generated executables, object files, or local IDE settings. Confirm that bundled audio, fonts, and other assets may be redistributed. No license is included.
