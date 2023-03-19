### This is the music only bot used on the [Dragons](https://discord.com/invite/bd8vUQd) Discord

## Features

- play tracks from youtube, spotify and soundcloud
- loop your searched tracks
- volume controll
- player dashboard
- active dev

## Requirements

- [at least Python Version 3.11](https://www.python.org/downloads/)
- [git](https://git-scm.com/)
- [a discord bot token](https://discord.com/developers/applications)
- [server hosting lavalink](https://github.com/freyacodes/Lavalink)
    - [a free list is here](https://lavalink.darrennathanael.com/)
- py-cord  `pip install py-cord`
- pycord-multicog `pip install pycord-multicog`
- pomice (removed the discord.py requirement) `pip install git+https://github.com/DTheIcyDragon/pomice`

# Initial setup

## Configuring Lavalink Servers for Discord Bots

This JSON file is a configuration file for a Discord bot that connects to Lavalink servers. The key represents the name of the node which is used only in the program. The values correspond to their respective variables used in the program.

Usage
To set up the Lavalink servers in the configuration file, follow these steps:

1. Open the JSON file in a text editor.
2. Add a new node to the JSON file by using the following format:

```json
"node_name": {
    "HOST": "ip_address_of_the_Lavalink_server",
    "PORT": port_number_of_the_Lavalink_server,
    "PASSWORD": "password_for_the_Lavalink_server",
    "SECURE": boolean_value_for_secure_connection,
    "SPOTIFY_ID": "spotify_client_id",
    "SPOTIFY_SECRET": "spotify_client_secret"
}
```

3. Replace the values in the above format with the actual values of your Lavalink servers and Spotify credentials.
4. Save the file.

Once the configuration file is set up, the Discord bot will use the specified Lavalink servers to play audio.

## Configure the config.py

```py
from pathlib import Path

DISCORD_TOKEN = "" # here you enter your discord token you got under 
                   # https://discord.com/developers/applications

DBPATH = Path("./data/main.sqlite")
DBFOLD = Path("./data/")
GUILDS = []        # here you enter the guild ids you want the bot to work on
```
