1. <a href="https://github.com/sheiddy/tedicross_modified">Vehicles Lost Tracker Bot</a>
2. <a href="https://github.com/sheiddy/map_bot">Mapper Bot</a>


# <a href="./vehtracker_bot.md">Vehicles Lost Tracker Bot</a>
<a href="https://github.com/sheiddy/tedicross_modified">Repo</a>
### Original Message (from telegram):

![image](https://github.com/user-attachments/assets/12bf555a-bdad-4515-b97e-01c5993df2bb)

### Forwared Message (to telegram):
![image](https://github.com/user-attachments/assets/783d2c89-d3a6-4978-af9a-6caa27363a3e)

### Translate & Add flavor text+apply filters:
![image](https://github.com/user-attachments/assets/b9877710-802b-4de0-a7cb-28f263728eb6)

Note: the `<@&1270820068187701298>` part of the string is for tagging the @VehLosses role on discord.

### Post on discord:
![image](https://github.com/user-attachments/assets/e13df4c1-3c8e-4b71-a519-1d679fd168e9)

INFO: Some telegram videos are too large and will not be uploaded to discord (Discord limitation)

### Post on twitter:
![image](https://github.com/user-attachments/assets/c525c026-fe90-40dc-bd5b-5f4cd1789761)

INFO: Twitter does not allow for more than 4 media (images or videos) to be posted at a time.

# <a href="./mapper_bot.md">Mapper Bot</a>:
<a href="https://github.com/sheiddy/map_bot">Repo</a>

### Usage:
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

![image](https://github.com/user-attachments/assets/02645370-76fe-46a8-a541-5c5b32e0743e)
