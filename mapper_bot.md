# Mapper Bot
A Discord bot that takes some GPS coordinates and returns a satellite picture at that location with the frontline/zone of control included from a custom map.

## Usage:
Usage example using slash commands (`/`).
* `/map lat long` Example: `/map 51.277166 34.925880`
* `/map lat, long` Example: `/map 51.277166, 34.925880`
* `/map lat long zoom_level` Example: `/map 51.277166 34.925880 17`
* `/map lat long zoom_level map_type` Example: `/map 51.277166 34.925880 17 uacontrolmap`

Usage example using exclamation mark commands (`!`).

* `!map lat long` ->  `!map 51.277166 34.925880`
* `!map lat, long` -> `!map 51.277166, 34.925880`
* `!map lat long zoom_level` -> `!map 51.277166 34.925880 17`
* `!map lat long zoom_level map_type` -> `!map 51.277166 34.925880 17 uacontrolmap`

 *Only* `map` *commands work with both* `!` *and* `/` *prefixes but the* `/` *commands are a bit sketchy when pasting entire coordinates on mobile.*

You can you use the command with minimum 2 inputs (latitude and longitude) and 1 or 2 optional: 
* `zoom_level` - higher the number, closer to the ground. `default = 12`
* `map_type` - control map selection. Currently there are 4 control maps: AMK Mapping, UAcontrolmap, Andrew Perpetua's map and  creamy_carice's map. You can view the available maps by using the `/maps` command. Specifying a different control map that is not in the list will return the default one `AMK Mapping`.

### Maps:
    `UAMap - uacontrolmap `
    `AP - Andrew Perpetua`
    `AMK - AMK Mapping (default)`
    `CCaprice - creamy_carice`


Different maps have different loading times. Wait a few seconds if it doesn't load immediately :joe_realShrug: 

List of commands:
* `!map`
* `/map`
* `/help`
* `/maps`

### Example:

  ![image](https://github.com/user-attachments/assets/02645370-76fe-46a8-a541-5c5b32e0743e)

### Installing and running the bot
   * Discord bot installation and token:
     1. Go to <a href="https://discord.com/developers/docs/intro">Discord's Developer Portal</a>
     2. Create a new application By going to Applications (left panel) => "New Application"=> name it and click "Create"
     3. Go to "Bot" on the left panel and under "Token" set on "Reset Token" button and save the bot token.
     4. Under the same Bot page as above, scroll down and enable "Public Bot", "Presence Intent" and "Message Content Intent".
        ![image height=20](https://github.com/user-attachments/assets/0166de31-c9de-44c0-9ae2-43092f9ac363)
     6. Add the bot to your server by going to "Installation" from the left tab and copy the Install Link and paste it in a new webpage (this will redirect you to discord with a prompt to add the bot).
   * Python bot:
     1. Have python installed
     2. Install the necessary libraries (selenium might not be mandatory):
        
        `pip install discord.py selenium geopy Pillow playwright`
     
     4. In the bot's python file (bot.py?, bot_claude.py?) add the bot token to the `TOKEN` object.
     5. Start the bot by running "python bot_claude.py"
        ![image](https://github.com/user-attachments/assets/49d40f21-a7ae-441f-b01d-28b1964e068d)
     6. The discord bot should come online now (you can verify by checking bot's profile on discord
        ![image](https://github.com/user-attachments/assets/999202b3-072a-4c4d-8b40-9953d5df4064)
     7. Typical output for a successful task when running the `!map` command:
        ![image](https://github.com/user-attachments/assets/50f38f81-3f08-4915-acb1-4cabd379aa13)



        
