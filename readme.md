# linux-discord-rpc config
personal config for [linux-discord-rpc](https://github.com/trickybestia/linux-discord-rich-presence/blob/main/doc/configs/all-in-one.sh)


**Variables**
```bash
CONF_DISCORD_APPID=<discord-application-id> # acquire from discord developer portal
```

**Running**
```bash
$ env CONF_DISCORD_APPID=<app-id> linux-discord-rpc --config /path/to/config
```

<hr>

### module: cmus
> get cmus playing song as status
> show "Not playing" if cmus is inactive
> additionally dynamically set large_image with cover image if possible

**Variables**
```bash
CONF_CMUS_DISCORD_TOKEN=<discord-user-token> # for uploading cover image assets
```

### module: sway focused window
> get current focused window as status
> show "Desktop" if no window was focused
