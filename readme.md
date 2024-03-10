# linux-discord-rich-presence config
personal config for [linux-discord-rich-presence](https://github.com/trickybestia/linux-discord-rich-presence/blob/main/doc/configs/all-in-one.sh)

![Profile](https://i.imgur.com/vYYjsUM.png)


**variables**
```bash
CONF_DISCORD_APPID=<discord-application-id> # acquire from discord developer portal
```

**running**
```bash
$ env CONF_DISCORD_APPID=<app-id> ... linux-discord-rich-presence --config /path/to/config
```

<hr>

### module: cmus
> show cmus currently playing song as status
> 
> show "Not playing" while cmus is inactive
>
> additionally set cover image as large_image and automatically remove unused assets to avoid the 300 limit

**variables**
```bash
CONF_CMUS_DISCORD_TOKEN=<discord-user-token> # for managing presence assets
```

### module: sway focused window
> set currently focused window as status
>
> show "Desktop" while no window is focused
