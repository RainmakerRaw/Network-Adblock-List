A small but flexible ABP format (Pi-Hole, AdGuard Home, uBO) blocklist for network adblockers. This list is intended as a supplement to [abp.oisd.nl](https://abp.oisd.nl).

Mostly it tidies up and catches a few subdomains missed by the main list. For example, the main OISD list has almost 200 entries each for various subdomains of doubleclick, firebase and so on. This list simplifies things and just blocks them outright with, for example, `*firebase*^` and `*doubleclick*^`. It also blanket-bans `*analytics*^`, `*metrics*^` and *`telemetry*^`, and in doing so catches a few domains missed by the main OISD list (like `client-telemetry.roblox.com`).

Please use this list however you wish. If there are any questions or problems, just open an [Issue](https://github.com/RainmakerRaw/Network-Adblock-List/issues). 

Thanks!
