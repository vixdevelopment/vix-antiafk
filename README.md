# vix-antiafk


A standalone anti-afk system script


## Installation
1. Place the `vix-antiafk` folder in your server `resources` directory.
2. Add `start vix-antiafk` to your `server.cfg`.
3. Edit `config.lua` to set `AFKMinutes` and `KickMessage`.
4. Restart your server or ensure the resource is started.


## Notes
- The client sends periodic heartbeats; the server uses the server-side clock to decide when to kick.
- Tweak `ClientHeartbeat` and `CheckInterval` to balance responsiveness vs server load.
- This is intentionally simple — you can extend it to log kicks, exempt certain identifiers/groups, or add admin commands.
