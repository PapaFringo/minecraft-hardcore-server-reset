Hardcore Auto-Reset Minecraft Server (Fabric)

This project provides a small Python script that automatically deletes the world folder and restarts the Minecraft server whenever a player dies — perfect for hardcore-style survival challenges on a Fabric server.

🚀 Server Start Command

Example command to start a Fabric Minecraft server:

java -Xmx2G -jar fabric-server-mc.1.21.6-loader.0.18.1-launcher.1.1.0.jar nogui

🧩 What the Script Does

Automatically launches your Minecraft server

Detects player deaths via server logs

Deletes the entire world folder on any player death

Restarts the server afterward

Stores all player death events

Provides a stats command to show all stored player statistics

📦 Installation & Usage
1. Prepare Your Server

Download a Minecraft server JAR (e.g., Fabric).

Copy your server launch command.

2. Set Up the Script

Place the hardcore.py script inside your server directory.

Run it:

python3 hardcore.py


Let the script start the server once completely.

Stop the server afterward.

❗ One-Time Initialization Step

On the first startup, Minecraft generates the world — but not in hardcore mode.
Therefore you must manually delete the world folder once before the hardcore loop can begin.

3. Edit Server Settings

Open your server.properties file and enable Hardcore mode:

hardcore=true


(You may adjust any other settings as needed.)

4. Start the Hardcore Loop

Run the script again.
Your server will now automatically reset the world and restart whenever a player dies.

📊 Player Statistics

The script stores:

Number of deaths per player

Timestamp of each death

Last session information

Use the console command:

stats


to display all collected player statistics at any time.
