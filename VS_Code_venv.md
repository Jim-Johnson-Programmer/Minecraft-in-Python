Below is a **clean, focused, VS Code–only quickstart** for brand‑new Python programmers. It’s written so you can drop it straight into onboarding docs or hand it to a student who has never touched a virtual environment before.

---

# 🐍 **Python Virtual Environment Quickstart (VS Code Edition)**

This guide teaches you how to run Python code in VS Code **using a virtual environment**, even if you’ve never used one before.

---

## 1. 📦 Install Python

Download Python from:

[https://www.python.org/downloads/](https://www.python.org/downloads/)

On **Windows**, make sure you check:

```
[✔] Add Python to PATH
```

---

## 2. 📁 Create Your Project Folder

Make a folder anywhere on your computer:

```
myproject/
```

Inside it, create a file:

```
myproject/app.py
```

Example content:

```python
print("Hello from VS Code!")
```

---

## 3. 🧰 Open the Folder in VS Code

1. Open VS Code
2. Go to **File → Open Folder**
3. Select your `myproject` folder

VS Code should now show your project in the Explorer panel.

---

## 4. 🛠️ Create a Virtual Environment (Inside VS Code Terminal)

Open the VS Code terminal:

- **View → Terminal**
- Or press **Ctrl+`**

Run one of the following commands **inside your project folder**:

### Windows

```
python -m venv venv
```

### macOS / Linux

```
python3 -m venv venv
```

This creates:

```
myproject/
    venv/
    app.py
```

---

## 5. ▶️ Activate the Virtual Environment

### Windows (PowerShell)

```
venv\Scripts\Activate.ps1
```

### Windows (CMD)

```
venv\Scripts\activate.bat
```

### macOS / Linux

```
source venv/bin/activate
```

You’ll know it worked when your terminal shows:

```
(venv)
```

---

## 6. 🧠 Tell VS Code to Use the venv Interpreter

VS Code needs to know which Python to use.

1. Press **Ctrl+Shift+P**
2. Type: **Python: Select Interpreter**
3. Choose the one that looks like:

```
./venv/bin/python
```

or

```
.\venv\Scripts\python.exe
```

VS Code is now fully connected to your virtual environment.

---

## 7. 📥 Install Packages (Inside the venv)

Example:

```
pip install requests
```

Check:

```
pip list
```

You’ll see only packages installed inside this project’s venv.

---

## 8. ▶️ Run Your Python Code

You can run your script in two ways:

### **A. Using the Terminal**

```
python app.py
```

### **B. Using the VS Code Run Button**

Open `app.py` and click:

```
▶ Run Python File
```

VS Code will run it using your selected interpreter (the venv).

---

## 9. 🧹 Deactivate When You’re Done

In the terminal:

```
deactivate
```

Your prompt returns to normal.

---

## 10. 🗑️ Resetting the Environment

If something breaks, just delete the folder:

```
venv/
```

Then recreate it with:

```
python -m venv venv
```

---

## 11. ⚡ Quick Troubleshooting

### VS Code is using the wrong Python

Use **Python: Select Interpreter** again.

### pip installs globally

You forgot to activate the venv.

### PowerShell won’t activate the venv

Run:

```
Set-ExecutionPolicy -Scope CurrentUser RemoteSigned
```

---

If you want, I can also prepare:

- a **print‑ready cheat sheet**
- a **classroom‑ready version** with diagrams
- a **VS Code + GitHub workflow guide**
- a **requirements.txt + deployment quickstart**

Just tell me what you want next.
