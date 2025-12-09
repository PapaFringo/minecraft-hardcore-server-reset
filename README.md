# Hardcore Auto-Reset Minecraft Server

This project provides a small Python script that automatically deletes the world folder and restarts the Minecraft server whenever a player dies.

---

## 🚀 Server Start Command

Example command to start a Minecraft server:

```bash
java -Xmx2G -jar xxx.jar nogui
```

---

## 🧩 What the Script Does

* Automatically launches your Minecraft server
* Detects which OS you are using - Linux (bash) or Windows
* Detects player deaths via server logs
* Deletes the entire `world` folder on any player death
* Restarts the server afterward
* Provides a `stats` command to show all stored player deaths

---

## 📦 Installation & Usage

### 1. Prepare Your Server

* Download a Minecraft server JAR
* Copy your server launch command

### 2. Set Up the Script

1. Place the `hardcore.py` script inside your server directory

2. Run it:

   * Double-click it **or**
   * Run via command line:

     ```bash
     python3 hardcore.py
     ```
3. The script will ask for the launch command

4. Let the script start the server once completely

5. Stop the server afterward

---

## ❗ One-Time Initialization Step

On the first startup, Minecraft generates the world — but **not** in hardcore mode.
Therefore you must **manually delete the `world` folder once** before the hardcore loop can begin.

---

### 3. Edit Server Settings

Hardcore mode will be set automatically.

---

### 4. Start the Hardcore Loop

Run the script again.
Your server will now automatically reset the world and restart whenever a player dies.

---

## 📊 Player Statistics

The script stores:

* Number of deaths per player

Type ingame:

```
stats
```

to display all deaths.

