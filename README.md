# Telegram Voice Chat Bot with Channel Support.

A Telegram Bot to Play Audio in Voice Chats With Youtube and Deezer support.
Supports Live streaming from youtube

```
Please fork this repository don't import code
Made with Python3
(C) @subinps
Copyright permission under MIT License
License -> https://github.com/subinps/MusicPlayer/blob/master/LICENSE

```

## Deploy to Railway #For free

[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/new/template?template=https%3A%2F%2Fgithub.com%2Fabrock00%2FMusicPlayer&envs=APP_ID%2CAPI_HASH%2CSESSION_STRING%2CCHAT%2CLOG_GROUP%2CADMINS%2CARQ_API%2CMAXIMUM_DURATION&APP_IDDesc=Get+From+my.telegram.org&API_HASHDesc=Get+from+my.telegram.org&SESSION_STRINGDesc=tgsession.infotelbot.com&CHATDesc=ID+of+Channel%2FGroup+where+the+bot+plays+Music+Link&LOG_GROUPDesc=Group+to+send+Playlist%2C+if+CHAT+is+a+Group+Link&ADMINSDesc=ID+of+users+who+can+use+admin+commands.&ARQ_APIDesc=Get+it+for+free+from+%40ARQRobot%2C+This+is+required+for+%2Fdplay+to+work&MAXIMUM_DURATIONDesc=Maximum+duration+of+song+to+play.%28Optional%29&MAXIMUM_DURATIONDefault=160)

NOTE: Make sure you have started a VoiceChat in your Group before deploying.
### Deploy to VPS

```sh
git clone https://github.com/subinps/MusicPlayer
cd MusicPlayer
pip3 install -r requirements.txt
# <Create Variables appropriately>
python3 main.py
```

# Vars:
1. `API_ID` : Get From my.telegram.org
2. `API_HASH` : Get from my.telegram.org
3. `BOT_TOKEN` : @Botfather
4. `SESSION_STRING` : Generate From here [![GenerateStringName](https://img.shields.io/badge/repl.it-generateStringName-yellowgreen)](https://repl.it/@subinps/getStringName)
5. `CHAT` : ID of Channel/Group where the bot plays Music.
6. `LOG_GROUP` : Group to send Playlist, if CHAT is a Group
7. `ADMINS` : ID of users who can use admin commands.
8. `ARQ_API` : Get it for free from [@ARQRobot](https://telegram.dog/ARQRobot), This is required for /dplay to work.
9. `STREAM_URL` : Stream URL of radio station or a youtube live video to stream when the bot starts or with /radio command. [Some Streaming Links](https://gist.github.com/subinps/293d0a117fa0b13da41871538f226956)
10. `MAXIMUM_DURATION` : Maximum duration of song to play.(Optional)
11. `REPLY_MESSAGE` : A reply to those who message the USER account in PM. Leave it blank if you do not need this feature. 
12. `ADMIN_ONLY` : Pass `Y` If you want to make /play and /dplay commands only for admins of `CHAT`. By default /play and /dplay is available for all.

- Enable the worker after deploy the project to Heroku
- Bot will starts radio automatically in given `CHAT` with given `STREAM_URL` after deploy.(24*7 Music even if heroku restarts, radio stream restarts automatically.)  
- To play a song use /play as a reply to audio file or a youtube link.
- Use /play <song name> to play song from youtube and /dplay <song name> to play from Deezer.
- Use /help to know about other commands.

**Features**

- Playlist, queue.
- Change VoiceChat title to current playing song name.
- Supports Live streaming from youtube
- Supports both deezer and youtube to search songs.
- Play from telegram file supported.
- Starts Radio after if no songs in playlist.
- Automatically downloads audio for the first two tracks in the playlist to ensure smooth playing
- Automatic restart even if heroku restarts.

### Note

```
Contributions are welcomed, But Kanging and editing a few lines wont make you a Developer.
Fork the repo, Do not Import code.

```
#### Support

Connect Me On [Telegram](https://telegram.dog/subinps_bot)

## Credits 
- [Dash Eclipse's](https://github.com/dashezup) for his [tgvc-userbot](https://github.com/callsmusic/tgvc-userbot).

