---
layout: post
title: How to make a Radio Bot on Telegram
subtitle: How to make a Radio Bot on Telegram with heroku 
tags: [Bot]
comments: true
---

# Telegram Radio Player V3


Telegram Bot to Play Radio/Music/YouTube Live on Channels or Group Voice Chats.

This is also the source code of the bot used to play
Radio in [AsmSafone](https://t.me/AsmSafone) Channels & Music in Groups [SafoTheBot](https://t.me/safothebot).

## Special features

- Playlists, queues, radio streams 24x7
- Support live streaming from youtube
- Start Radio after if there is no song in playlist
- Automatic playback even if heroku restarts
- Show current audio playback position
- Control with buttons and commands
- Download songs from youtube as audio
- Automatically downloads audio for the first two tracks in a playlist to ensure smooth playback

## Apply to Heroku (Easy Way)



[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/AsmSafone/RadioPlayer/tree/V3.0) 
NOTE: Make Sure You Have Started Voice Chat On Your Channel/Group Before Deploy!

## Heroku Vars:
1. `API_ID` : Get Dari my.telegram.org
2. `API_HASH` : Get Dari my.telegram.org
3. `BOT_TOKEN` : Get Dari @Botfather
4. `SESSION_STRING` : Earn From [@genStr robot](http://t.me/genStr_robot).
5. `CHAT` : ID of the Channel/Group where the bot plays Music/Radio.
6. `LOG_GROUP` : Group to send Playlist, if CHAT is Group.
7. `ADMINS` : User IDs that can use admin commands.
8. `STREAM_URL` : The streaming URL of a radio station or youtube live video to stream when the bot is started or with the /radio command.
9. `MAXIMUM_DURATION` : Maximum length of song to play. (Optional)
10. `REPLY_MESSAGE` : Reply to those who messaged the USER account in PM. Leave it blank if you don't need this feature.
11. `ADMIN_ONLY` : Pass Y If you want to make command /play only for admin CHAT. By default /play is available to all.

- Unlock workers after deploying projects to Heroku.
- The bot will start the radio automatically in the given `CHAT` with the given `STREAM_URL` after deployment.
- 24x7 music even if heroku restarts radio stream restarts automatically.
- To play a song use /play as a reply to the audio file or youtube link or use /play [song name].
- To download audio, you can use [@SafoneMusicBot](http://t.me/SafoneMusicBot) or `/song` command to the bot.
- Use `/help` to know about other commands & their usage.

## Requirements

- Python 3.6 or higher.
- A
   [Telegram API Key](https://docs.pyrogram.org/intro/quickstart#enjoy-the-api)
   and Telegram accounts.
- [FFmpeg Python](https://www.ffmpeg.org/)
- Telegram [Session String](http://t.me/genStr_robot) from the account.
- Userbot Must Be Admin In Channel or Group.
- Must Start Voice Chat On Channel/Group Before Running Bot.

## Run On VPS (Hard Road)

```sh
$ git clone -b V3.0 https://github.com/AsmSafone/RadioPlayer
$cd RadioPlayer
$ sudo apt-get install python3-pip ffmpeg
$ pip3 instal -U pip
$ pip3 install -r requirements.txt
# <create variables correctly>
$ python3 main.py
```


## Licence
``` sh
RadioPlayer Telegram Voice Chat Bot
Copyright (c) 2021 Asm Safone

This program is free software: you can redistribute it and/or modify it
it is under the terms of the GNU Affero General Public License as published by
Free Software Foundation, either version 3 of the License, or
(according to your choice) a newer version.

This program is disseminated in the hope that it will be useful,
but WITHOUT ANY WARRANTY; even without the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. see
GNU Affero General Public License for more details.

You should have received a copy of the GNU Affero General Public License
along with this program. If not, see <https://www.gnu.org/licenses/>
```
