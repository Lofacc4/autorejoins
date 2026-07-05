# Auto Rejoin

A Minecraft Fabric mod that helps you never lose your spot on a multiplayer server again.

## Why We Made This

We got tired of the same thing happening over and over - you're deep in a survival world with friends, building something cool, and then Minecraft crashes. Or Windows decides it's update time. Or your internet drops for a second. When you come back, the server's still there but you've lost your flow.

Vanilla Minecraft doesn't help you get back quickly. You have to manually find the server in your list, wait for it to ping, double-click... it's annoying. So we built a toolkit that does it for you.

## What It Does

- **Server Bookmarks** - Star your favorite servers for quick access
- **Connection History** - See where you've played recently with timestamps
- **Server Status** - Know if a server is online before joining
- **Reconnect Shortcuts** - Shortcuts saved to your startup so you can jump back in after a crash
- **Auto Backups** - Never lose your server list
- **Ping Utility** - Accurate latency numbers

## How It Works

Just drop the mod in your mods folder. It runs silently in the background - no commands to remember, no UI to configure unless you want to. Everything is set up in `config/auto-rejoin.properties` if you want to tweak things.

When you join a server, the mod remembers it. When you disconnect or crash, your rejoin shortcut is waiting for you.

## Compatibility

- Fabric Loader 0.16+
- Minecraft 1.20+
- Client-side only - no server install needed
- Works with Lunar Client, Prism, MultiMC, vanilla launcher

## Configuration

All settings in `config/auto-rejoin.properties`:

| Setting | Default | Description |
|---|---|---|
| saveShortcuts | true | Save reconnect shortcuts |
| trackHistory | true | Track connection history |
| checkStatus | true | Check server status |
| maxBookmarks | 50 | Max bookmarks to keep |
| pingTimeout | 2000 | Ping timeout in ms |
| autoBackup | true | Auto-backup server lists |
