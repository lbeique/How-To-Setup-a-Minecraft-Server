---
layout: default
title: Troubleshooting
nav_order: 6
---

| **Symptoms** | **Probable Cause** | **Action** |
| ------------ | ------------------ | ---------- |
| Unable to see folder. | Hidden view is disabled | If you can't find the AppData folder in your File Explorer, click View at the top of the folder window and make sure "Hidden Items" is checked. |
| Mod pack gives an error | Mod pack may be editing the same content as another mod pack. | Two mods that effect zombie mods may interfere with one another. It is best to pick only one mod from the two to avoid conflict. |
| None of the mods are loading | Not using correct server jar | Ensure you are running the Forge minecraft server and not the original <minecraft_server.jar> |
| Can't interact with the game near the player spawn. | There is a spawn protection setting on the server. | Go into the server.properties file and change the spawn-protection value from 16 to 0. |
| Can't connect to Game Services. | The Mojang Studio servers might be down. | Check the [Mojang Status Twitter](https://twitter.com/MojangStatus) to see if the servers are down. Otherwise, check your firewall and/or antivirus and make sure to allow the game's connection. |
| The Server failed to start. | This is common if the eula is still set to false. | Open the eula.txt file and change the line eula=false and replace it with eula=true. |
| Other users can not find my server | The server might not be running, or the IPs/Ports were not properly entered into the configuration files. | Before another player can join the server, it needs to be running in the background. It is also possible that the server.properties file is missing the server-ip value. Or finally, it is possible that the users were given the wrong IP address, make sure it is the one you found on [whatismyipaddress.com](https://whatismyipaddress.com/). |
