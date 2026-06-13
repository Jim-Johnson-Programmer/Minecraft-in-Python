# Minecraft-in-Python

Simple 3D Minecraft-style project built with the Ursina game engine.

## Prerequisites

- Python 3.10 or newer
- `pip`
- Windows PowerShell or Command Prompt

## Project layout

The game entry point is `python_minecraft/game.py`.

Important: run the game from the `python_minecraft` directory so the `Assets/...` paths resolve correctly.

## Create and activate a virtual environment

From the project root:

```powershell
cd .\Minecraft-in-Python
python -m venv .venv
```

Activate the virtual environment in PowerShell:

```powershell
.\.venv\Scripts\Activate.ps1
```

If you are using Command Prompt instead:

```bat
.venv\Scripts\activate.bat
```

## Install dependencies

With the virtual environment activated:

```powershell
python -m pip install --upgrade pip
python -m pip install ursina
```

## Run the game

Change into the folder that contains the game script and assets, then start the game:

```powershell
cd .\python_minecraft
python .\game.py
```

## Deactivate the virtual environment

When you are done:

```powershell
deactivate
```

## Troubleshooting

- If `Activate.ps1` is blocked in PowerShell, run:

```powershell
Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass
```

Then activate the virtual environment again.

- If the game opens with missing assets or textures, make sure you started it from the `python_minecraft` folder, not from the repository root.
