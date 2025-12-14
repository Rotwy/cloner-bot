# Discord Server Cloner

A Python tool for cloning Discord servers using self-bot functionality.

## ⚠️ Disclaimer

This tool uses self-bot functionality which is against Discord's Terms of Service. Use at your own risk. The creators are not responsible for any accounts that get banned or restricted.

## Features

- Clone server roles
- Clone server channels (text and voice)
- Clone server categories
- Clone server emojis
- Clone server icon and name

## Requirements

- Python 3.6+
- Discord.py (self-bot version)
- Colorama
- Psutil

## Installation

1. Install the required packages:
```
pip install discord.py-self colorama psutil
```

2. Clone or download this repository

## Usage

1. Run the script:
```
python main.py
```

2. Enter your Discord account token when prompted
3. Enter the ID of the server you want to copy from
4. Enter the ID of the server you want to copy to

## How It Works

The tool connects to Discord using your account token and performs the following actions:
1. Edits the destination server's name and icon to match the source server
2. Deletes all existing roles in the destination server (except @everyone)
3. Deletes all existing channels in the destination server
4. Recreates all roles from the source server in the destination server
5. Recreates all categories from the source server in the destination server
6. Recreates all channels (text and voice) from the source server in the destination server

## Known Issues

1. The tool doesn't preserve channel history or messages
2. Some permission overwrites may not be copied correctly
3. User-specific settings are not transferred
4. Bans and invites are not copied

## Potential Improvements

1. Add error handling for rate limits
2. Implement backup/restore functionality
3. Add option to selectively clone specific elements
4. Improve permission mapping between roles

## Legal Notice

This tool is for educational purposes only. The misuse of this tool may result in your Discord account being permanently banned. The developers assume no liability and are not responsible for any misuse or damage caused by this tool.