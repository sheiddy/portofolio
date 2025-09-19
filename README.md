Following is a list of some of my projects, ordered by date, most recent first.

1. Bots Updates Bot
2. Air Raid Alert Bot
3. [Vehicles Lost Tracker Bot](#vehicles-lost-tracker-bot)
4. [Mapper Bot](#mapper_bot)
5. [CSGO Trader Bot](#csgo_traderbot)
6. [ESP Smart Home](#esp_smarthome)
7. [Tarkov Companion](#tarkovcompanion)
8. [ARK Webshop](#ark_webshop)
9. [Soccer stats retrieval](#soccer_stats)


# Bots Updates Bot
This bot will send update messages for all of our bots on our [discord server](https://discord.gg/ZDankYjn).
Example message below:
<img width="533" height="246" alt="image" src="https://github.com/user-attachments/assets/ce6d5171-e753-4e39-875b-29a40d5793b9" />


# Air Raid Alert Bot
Discord notifications of air raids alerts in Ukraine. Done in n8n. Will send city/region update and oblast raid alerts with an associated oblasts map.  
V1:  
![image](https://github.com/user-attachments/assets/c04924b6-5499-4af4-b5e6-956fb03d0986)  
V2:  
![image](https://github.com/user-attachments/assets/c867008e-e8e3-4f8d-aa25-b6d85e312912)  
Notifications message:  
![image](https://github.com/user-attachments/assets/dddb0408-59e4-44cd-86cb-433d406ce135)

<img width="483" height="495" alt="image" src="https://github.com/user-attachments/assets/f74d3284-d257-49e2-862c-b0370b85e032" />




# <a id="vehicles-lost-tracker-bot" href="./vehtracker_bot.md">Vehicles Lost Tracker Bot</a>
<a href="https://github.com/sheiddy/tedicross_modified">Repo</a>

This is a bot that lurks on telegram servers and gets messages about finding a new vehicle that is destroyed or damaged in the Ukraine - Russia war (2022-).
The bot will get the messages from another (telegram) bot that forwards the messages found to a private telegram server that we have access to. The bot will parse the message and translate it and then:
1. Forwards the message including photos/videos to a discord server and
2. Takes the message including up to 4 photos/videos and makes a post on <a href="https://x.com/LostWarBot">twitter</a> about it.

<img width="468" height="560" alt="image" src="https://github.com/user-attachments/assets/a36422f9-6aea-43f4-98ab-77eec644272d" />


### Original Message (from telegram):

<img width="437" height="413" alt="image" src="https://github.com/user-attachments/assets/3bbdad17-f862-4de2-9b76-558affaca88f" />

### Forwared Message (to telegram):
<img width="433" height="390" alt="image" src="https://github.com/user-attachments/assets/3f24ca3e-a47d-405e-a004-7a3e7e840525" />

### Translate & Add flavor text+apply filters:
<img width="1235" height="189" alt="image" src="https://github.com/user-attachments/assets/02f3a63d-7af7-4975-ac82-5a7fbe511b76" />

Note: the `<@&1270820068187701298>` part of the string is for tagging the @VehLosses role on discord.

### Post on discord:
<img width="510" height="392" alt="image" src="https://github.com/user-attachments/assets/a6ac536a-f75b-4ea9-9483-90e294c51ca3" />

INFO: Some telegram videos are too large and will not be uploaded to discord (Discord limitation)

### Post on twitter:
<img width="532" height="397" alt="image" src="https://github.com/user-attachments/assets/1b5c46bc-e8b8-482b-bfbf-6780ca6740db" />

INFO: Twitter does not allow for more than 4 media (images or videos) to be posted at a time.

<!----------------------------------------------------------------------------------------------------------------->

# <a id="mapper_bot" href="./mapper_bot.md">Mapper Bot</a>:
<a href="https://github.com/sheiddy/map_bot">Repo</a>

This is a bot that once added to a discord server, will take a map command with GPS coordinates and it will return a satelite photo at the specified location with the ukrainian/russian frontline shown on it (if close enough).

The bot includes 4 different sources for the frontline and can be specified by the user (default one is `AMK`). The bot can also take a zoom parameter.

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
    `CCaprice - creamy_caprice`


Different maps have different loading times. Wait a few seconds if it doesn't load immediately :joe_realShrug: 

List of commands:
* `!map`
* `/map`
* `/help`
* `/maps`

<img width="485" height="389" alt="image" src="https://github.com/user-attachments/assets/f1c0147d-6170-447e-85ef-943affb18b3c" />

<img width="1254" height="872" alt="image" src="https://github.com/user-attachments/assets/67604d31-7cda-42e2-a188-2f3c2f90e383" />


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

<img width="3637" height="1790" alt="image" src="https://github.com/user-attachments/assets/7af3784d-459e-4d2a-ae33-881eb335ad33" />

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

