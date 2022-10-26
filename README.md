NW_Timerbot
--------------

A free discord bot to call the respawn time of wars in the NEW WORLD game.

![](https://github.com/BigChicChicken/NW_TimerBot/blob/main/demo.gif "Demo")

Installation
--------------

[Install FFmpeg](https://ffmpeg.org/)

[Install Python](https://www.python.org/)

[Install NodeJs](https://nodejs.org/)

[Install Yarn](https://yarnpkg.com/)

Download/Clone this repository.

Step by step for Windows
--------------
1. Install FFmpeg
- Download [FFmpeg](https://www.gyan.dev/ffmpeg/builds/ffmpeg-git-full.7z).
- Extract the content.
- Rename the folder extracted to `ffmpeg`.
- Copy/Paste the folder into `C:\`.
- Edit the system environment variables and add the path `C:\ffmpeg\bin`.

2. Install Python
- Download [Python](https://www.python.org/ftp/python/3.11.0/python-3.11.0-amd64.exe).
- Launch the `.exe` file and don't forget to tick the option "**Add python.exe to PATH**"

3. Install NodeJs
- Download [NodeJs](https://nodejs.org/dist/v18.12.0/node-v18.12.0-x64.msi).
- Launch the `.msi` file.

4. Install Yarn
- Download [Yarn](https://objects.githubusercontent.com/github-production-release-asset-2e65be/49970642/ff4764f9-bcd8-485c-af33-9030f7fa1fdb?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIWNJYAX4CSVEH53A%2F20221026%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20221026T190549Z&X-Amz-Expires=300&X-Amz-Signature=e20fa7da8b31b0562b1743ab68736d2e8e1af0529752f393b8980202c07cd3de&X-Amz-SignedHeaders=host&actor_id=40992270&key_id=0&repo_id=49970642&response-content-disposition=attachment%3B%20filename%3Dyarn-1.22.19.msi&response-content-type=application%2Foctet-stream)
- Launch the `.msi` file.

5. Install Bot
- Download this [repository](https://codeload.github.com/BigChicChicken/NW_TimerBot/zip/refs/heads/main).
- Extract the content.
- Modify the file `.env` file like in [Configuration](https://github.com/BigChicChicken/NW_TimerBot#configuration).
- Open a command console into the root directory.
- (*Optional*) You can run these commands to check previous installations:
  - `ffmpeg --version`
  - `python --version`
  - `node --version`
  - `yarn --version`
- Run the command `yarn install` to install dependencies.
- Then the command `yarn prod` to start bot.

Configuration
--------------
In the `.env` update values with your data, like the example.

Under **BOTS**, you will have to define:
- **name**: The name of the bot, used to create an associated log file.
- **lang**: Choose the bot voice language. (available fr|en)
- **token**: The token to connect to your discord api bot. [Dev Portal](https://discord.com/developers)
- **voiceChannelId**: The id of the channel where the bot connects.
- **textChannelId**: The id of the channel where the control buttons will be sent.

Under **MASTER_BOT**, you will have to define:
- **token**: The token to connect to your discord api bot. [Dev Portal](https://discord.com/developers)
- **textChannelId**: The id of the channel where the control buttons will be sent.

Exemple:
```dotenv
BOTS: '[
    {
        "name":"MyFirstBot",
        "lang": "en",
        "token":"my_first_bot_key",
        "voiceChannelId":"my_first_voice_channel_id",
        "textChannelId":"my_text_channel_id"
    },
    {
        "name":"MySecondBot",
        "lang": "en",
        "token":"my_second_bot_key",
        "voiceChannelId":"my_second_voice_channel_id",
        "textChannelId":"my_text_channel_id"
    }
]'
MASTER_BOT: '{
    "token":"my_master_bot_key",
    "textChannelId": "my_text_channel_id"
}'
```

USAGE
----------

Under the root folder of this repository, launch the following commands:
- `yarn install` : Install all necessary dependencies.
- `yarn prod` : Turn on bots.

Now the bots are ready to help you win your future wars. ⚔️

![](https://github.com/BigChicChicken/NW_TimerBot/blob/main/screenshot.png "Screenshot")

License
----------

This is completely free and released under the [MIT License](https://github.com/BigChicChicken/NW_TimerBot/blob/main/LICENSE).
