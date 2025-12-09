Hardcore Auto-Reset Minecraft Server

This project provides a small Python script that automatically deletes the world folder and restarts the Minecraft server whenever a player dies.



🚀 Server Start Command

Example command to start a Minecraft server:

java -Xmx2G -jar xxx.jar nogui



🧩 What the Script Does

Automatically launches your Minecraft server

Detects player deaths via server logs

Deletes the entire world folder on any player death

Restarts the server afterward

Provides a stats command to show all stored player deaths



📦 Installation & Usage
1. Prepare Your Server

Download a Minecraft server JAR

Copy your server launch command.

2. Set Up the Script

Place the hardcore.py script inside your server directory.

Run it:

double click or python3 hardcore.py

Let the script start the server once completely.

Stop the server afterward.



❗ One-Time Initialization Step

On the first startup, Minecraft generates the world but not in hardcore mode.
Therefore you must manually delete the world folder once before the hardcore loop can begin.

3. Edit Server Settings
(hardcore will be set automatically)

4. Start the Hardcore Loop

Run the script again.
Your server will now automatically reset the world and restart whenever a player dies.



📊 Player Statistics

The script stores:

Number of deaths per player

Use the console command:

stats

to display all collected player statistics at any time.
