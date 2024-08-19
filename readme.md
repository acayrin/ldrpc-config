# linux-discord-rich-presence config
personal config for [linux-discord-rich-presence](https://github.com/trickybestia/linux-discord-rich-presence)

![Demo](https://i.imgur.com/vYYjsUM.png)

**requirements**
```
jq
```

**variables**
```bash
CONF_DISCORD_APPID=<int> # app id, acquire from discord developer portal <required>
CONF_DISCORD_USER_TOKEN=<str> # user token, for interacting with the discord user api, acquire from a browser's Dev tools [optional]
CONF_INTERVAL=<int> # interval in seconds between each state update, default to 5s [optional]
```

**running**
```bash
$ env CONF_DISCORD_APPID=<app-id> ... linux-discord-rich-presence --config /path/to/config
```

<hr>

### module: mpris
show current playing media as status

additionally upload thumbnails (if any) to discord directly and display them as large_image

**requirements**
```
playerctl, imagemagick, ffmpeg
```

**variables**
```bash
CONF_MPRIS_PLAYER=<str> # which mpris player should be used, default to Music Player Daemon [optional]
CONF_MEDIA_PATH=<str> # path to media directory, mostly for Music Player Daemon [required for MPD]
```

### module: wayland focused window
show current focused window as status

show "Desktop" while no window is focused

only ``Sway`` and ``Hyprland`` is supported
