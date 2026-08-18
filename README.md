# Colab-Minecraft-Server
A simple script to create a Minecraft server in google colab



Basic Setup:

# ALWAY WAIT TILL CONSOLE GIVES AN OUTPUT!!
1. Run the first cell containing the google drive mount code. This is necessary as colab sessions reset and will delete all your data. Upon running, you will be prompted to give google colab access to google drive. Select all and click ok.
2. Then run the second cell. This is the main server setup cell. It downloads the latest minecraft version, the latest java version and the latest playit.gg version.
3. After running the second cell, wait a bit. Eventually, you will be given a "Claim URL"
4. Click on it and sign into your playit.gg account and claim the agent.
5. Set a name and create a tunnel
6. It will give you an ip that you can then use to connect.
7. After this run the third cell. You are looking for something along the lines of

MINECRAFT
14826 java -Xms2G -Xmx4G -jar server.jar nogui

PORT: 25565
LISTEN 0      4096               *:25565            *:*    users:(("java",pid=14826,fd=64))       

PLAYIT
15015 /content/playit

GOOGLE DRIVE
Drive: MOUNTED

SERVER ON DRIVE
Server backup: PRESENT

PLAYIT CONFIG
Playit config backup: PRESENT

BACKUP PROCESS
15012 bash /content/minecraft-backup.sh
WORLD
World backup: PRESENT

9. Once it says this, you are good to go and can connect to your server.
10. After about 10 minutes run the 4th cell and ensure that the backup system is working. It takes a backup every 10 mins, keeping the last 5 so that if you need to reroll, you can.

Overall, if you liked this, then please let me know :D
If you have any questions, dm me on discord (thegwimweeper)
