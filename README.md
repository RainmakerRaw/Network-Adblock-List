A small but flexible ABP format (Pi-Hole, AdGuard Home, uBO) blocklist for network adblockers. This list is intended as a supplement to [abp.oisd.nl](https://abp.oisd.nl). I wrote this for my own use, ostensibly to be used with OISD in AdGuard's Hostlist Compiler. Unfortunately, the compiler's `Compress` function still isn't working as I wished to compact the two lists down to one, smaller, inclusive list. For now, this is my list of custom rules as added to my AdGuard Home DNS server.

Mostly it tidies up and catches a few subdomains missed by the main list. For example, the main OISD list has almost 200 entries each for various subdomains of doubleclick, firebase and so on. This list simplifies things and just blocks them outright with, for example, `||*firebase*^` and `||*doubleclick*^`. It also blanket-bans `||*analytics*^`, `||*metrics*^` and `||*telemetry*^`. In doing so, catches a few domains missed by the main OISD list, like `||client-telemetry.roblox.com`.  

I have found that, in daily use on a moderate home network, over 80 to 90% of my DNS blocks are from this small list alone. Please use this list however you wish. If there are any questions or problems, just open an [Issue](https://github.com/RainmakerRaw/Network-Adblock-List/issues) or fork. 

Thanks!
