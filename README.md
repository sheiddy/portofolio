1. [Vehicles Lost Tracker Bot](#vehicles-lost-tracker-bot)
2. [Mapper Bot](#mapper_bot)
3. [Trader Bot](#csgo_traderbot)
4. [ESP Smart Home](#esp_smarthome)
5. [Programu Lu Nicu](#programulunicu)
6. [Tarkov Companion](#tarkovcompanion)
7. [ARK Webshop](#ark_webshop)
8. [Soccer stats retrieval](#soccer_stats)


# <a id="vehicles-lost-tracker-bot" href="./vehtracker_bot.md">Vehicles Lost Tracker Bot</a>
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

<!----------------------------------------------------------------------------------------------------------------->

# <a id="mapper_bot" href="./mapper_bot.md">Mapper Bot</a>:
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

<!----------------------------------------------------------------------------------------------------------------->

# <a id="csgo_traderbot" href="./csgo_traderbot.md">CS:GO Trader Parser</a>:
<a href="https://github.com/sheiddy/CSGO_TraderParser">Repo</a>

Trade Parser bot for CSGOLounge and Dota2Lounge. It parses the entire website for trades that are favorable for us.

Ex(real scenario): their $84 CS:GO knife for our $75 knife. It basically gets all the items from all trades on the website and searches the price for that item on the steam community market returning favorable trades.

The program can search for particular items on the website instead of the entire website by checking the "Custom Lounge URL" togglebox. On european country, the website doesn't work. This can be bypassed by checking the "Lounge Proxy?" togglebox. It will parse proxys from the internet and then test and use them to access the website. [UPDATE 2022: the website is now accessible again from European countries]

The parser will not work anymore and has been discontinued. The website has changed the layout and has also removed the trading part of the website (you can only bet on the website now).

![image](https://user-images.githubusercontent.com/9354674/195376428-9d66ad58-5c8e-4556-b84b-fc09eb720f56.png)

Yellow = Separates the left side for the right side of each trade.

Red = Separates each trade.


Favorable trades will appear in green.

Trade link = Lounge trade link.

Item Name

Item Price = Price parsed from steam community.

Item Link = Link for each item on the steam community market.

<!----------------------------------------------------------------------------------------------------------------->

# <a id="esp_smarthome" href="./esp_smarthome.md">ESP Smart Home (WIP)</a>:
<a href="https://github.com/sheiddy/ESP_SmartHome">Repo</a>

Smart house interface using multiple ESP8266 across different rooms, with various sensors.

![image](https://github.com/sheiddy/ESP_SmartHome/assets/9354674/ed36b303-d84b-4073-b87d-57c090e39d6f)

<!----------------------------------------------------------------------------------------------------------------->

# <a id="programulunicu" href="./programulunicu.md">Programu' Lu' Nicu</a>:
<a href="https://github.com/sheiddy/ProgramuLuNicu">Repo</a>

Does a bunch of stuff suited for me, or stuff that I need/liked to build.

* Crypto Tab
  * Periodically fetches crypto prices (BTC + ETH only atm) and displays them on separate user control. Pic is for demo only with random values (API limitations).
![image](https://github.com/sheiddy/ProgramuLuNicu/assets/9354674/4864887a-c8f9-4388-bf51-1cd06acf8424)


 * Tarkov
  * Helpers for tarkov. For example, showing scavs and bosses HP on each  body part, showing various stats from selected scav.  
![image](https://github.com/sheiddy/ProgramuLuNicu/assets/9354674/934b1cde-9079-4bba-9a4f-984f02a97e14)

* ESP Tab
  * Interface for a ESP to connect to.
  * Depending on implementation, it can do one of the following:
    * Take data and events trough a ESP8266 D1 Mini from a PIR sensor and send notification to server (=PC running this program) and also plots the temp. Example:
![image](https://github.com/sheiddy/ProgramuLuNicu/assets/9354674/545a295f-5854-480a-9c76-2e42c016a8df)
    * Take data and events trough a ESP8266 D1 Mini from various greenhouse sensors (soil humidity, temperature, light). Still under development.


    * For the ESP D1 with a mini OLED display, use this configuration:
![image](https://github.com/sheiddy/ProgramuLuNicu/assets/9354674/b0f0fa6b-25da-4104-b54a-e969d0181c62)


* WW3 Tab
  * Will scrap the oryx website for all the lost equipment, for both the Ukraine and Russian side.
  * Takes data, parses it and uploads it to  ftp://win6042.site4now.net/lost_equipment_russia.html and ftp://win6042.site4now.net/lost_equipment_ukraine.html
  * Shows parsed and manipulated data to the WW3 tab and split onto those 2 countries. The update buttons will update the database with the latest losses from oryx.
![image](https://github.com/sheiddy/ProgramuLuNicu/assets/9354674/f8aad7a2-ab59-4cbf-b417-f21d64ccdeb8)


* ML Stuff development is paused ATM. Last time it was using quite a bit of CPU (this is not the reason for development pause tho).
 ![image](https://github.com/sheiddy/ProgramuLuNicu/assets/9354674/8006be5e-3fc3-4924-b559-09aeed72ed0c)

<!----------------------------------------------------------------------------------------------------------------->

# <a id="tarkovcompanion" href="./tarkovcompanion.md">Tarkov Companion</a>:
<a href="https://github.com/sheiddy/TarkovCompanion">Repo</a>

Tarkov Unofficial Companion

Price List Tab:
![image](https://user-images.githubusercontent.com/9354674/195537779-0074c859-268e-490b-8139-115b78fc0c93.png)

Barter Tab:
![image](https://user-images.githubusercontent.com/9354674/195537839-3c959c37-8c32-4c13-a4ad-4e7bb8de3fe7.png)
![image](https://user-images.githubusercontent.com/9354674/195537890-79258cd6-7033-4f1e-b21a-e828632b1e39.png)

Quests Tab:
![image](https://user-images.githubusercontent.com/9354674/195603182-94b10d09-cef0-4990-8f52-a32b7093ae60.png)

<!----------------------------------------------------------------------------------------------------------------->

# <a id="ark_webshop" href="./ark_webshop.md">ARK Webshop</a>:
<a href="https://github.com/sheiddy/Ark_WebShop">Repo</a>

Web Tool For ARK Shopping

[Discontinued]

 You can buy and sell any item directly to us. The software behind will automatically calculate the price. Easy and simple to use, select what item you want to buy, the quantity you want to buy and what items you are willing to exchange.
 Everytime an order is placed, we receive an e-mail with all the order details.
 
 Note: The shops takes commission on every transaction and is displayed before placing the order.
 
![image](https://user-images.githubusercontent.com/9354674/195377595-a67716ec-6cc0-4a63-a73b-5bf9294ca5a1.png)

![image](https://user-images.githubusercontent.com/9354674/195377790-546e65d4-cf8d-43f0-acb4-b5c90ca2f7ff.png)

![image](https://user-images.githubusercontent.com/9354674/195377827-04c96357-63a6-4a4f-ac45-e49a44258dc2.png)

![image](https://user-images.githubusercontent.com/9354674/195377857-b96463da-5513-446c-80d1-164b2830b557.png)

<!----------------------------------------------------------------------------------------------------------------->

# <a id="soccer_stats" href="./soccer_stats.md">Soccer Stats Retrieval</a>:
<a href="https://github.com/sheiddy/Soccer_Stats_Retrieval">Repo</a>

Gets all matches from soccerstats.com for the selected day that have not yet started. 
For each match found, it parses a set of data and passes them trough a self-made algorithm that returns matches that are worth betting on. 
Optionally, the "Parse Odds", when enabled, will search for those matches on flashscore.com and return their respective odds.

The website has been discontinued due to me a combination of me losing interest in sports betting, the introduction of cookies and other.

![image](https://user-images.githubusercontent.com/9354674/195376037-f3dd4edc-6d4f-40dc-bbde-4b79216d6984.png)

![image](https://user-images.githubusercontent.com/9354674/195376066-6c2e7b43-2144-4931-9e3a-a55a394b0d4c.png)

![image](https://user-images.githubusercontent.com/9354674/195376096-7acdd8c0-30e5-4233-a1ad-3fcb6df63db8.png)

![image](https://user-images.githubusercontent.com/9354674/195376131-a7365a23-0c58-408d-a4cb-ba74eac9e595.png)

![image](https://user-images.githubusercontent.com/9354674/195376157-6004cebd-7278-421a-8e23-2cfb3cad2027.png)

