# Simple Discord Bot Template

## About
This is a rather simple Discord bot built on [node.js](https://nodejs.org) using the [Discord.js](https://github.com/hydrabolt/discord.js) api.


## Installation
For starters you need [Node.js](https://nodejs.org) and you'll want the current version. **8.0.0 or newer is required.** 

Once you're sure you have node.js open the folder all the files are located and `shift + right click` > `Open command window here`.
You'll then want to run the following command
```
npm install
```
Ignore any warnings about unmet peer dependencies, as they're all optional from Discord.js.

### Setup Bot
Rename `config.example.json` to `config.json` and inside it you'll want to replace the token in there with your bot token that you get from [Discordapp Dev](https://discordapp.com/developers/applications/me). If you don't already have an app in there, create one. then press the button to turn the app into a bot user. `click to reveal` your Token and paste that into the config.json **Do NOT share this with anyone**
*While you're in there copy down your "Client ID", you'll need it later.*

Next you'll want to put your owner ID in the config.json. to get that, enable **Developer Mode** in discord under `Settings > Appearance > Advanced > Developer Mode`. After that you can just right click your username and **Copy ID**.

Set whatever **Prefix** you'd like in there while you're at it. *The prefix is the character you'll type before a command.*

If all went well you should be able to run **Normal Start.bat** and see "Bot is online!" in the console window.

### Invite Bot
Remember that "Client ID" I asked you to write down for later, above? Well we're gonna use that now to generate an invite link for your bot.

You can use a [Discord Permissions Calculator](https://discordapi.com/permissions.html) or just do what I do and give your bot all permissions by default using 
```
https://discordapp.com/oauth2/authorize?client_id=############&scope=bot&permissions=2146958591
```
*Replace the ############ with your Client ID*

Then going to the link will ask you what server you want the bot on. I think you can manage that part.

### Optional Part [Always Online Bot]
You might notice there's some files called **PM2 Start.bat**, **PM2 Stop.bat** and **PM2 Console Log.bat**. These are for using PM2 which is a package that keeps node programs running after they've crashed or something.
If you don't care about this, delete those 3 files. However if you do want to use this, open a command window again like before `shift + right click` > `Open command window here`. then type 
```
npm install -g PM2
```
then instead of using **Normal Start.bat** you'll have to click **PM2 Start.bat** and to see the log click **PM2 Console Log.bat**. you can have all these windows closed and your bot will still be running in the background as long as it's powered. To stop you click **PM2 Stop**

### Enjoy
Hopefully by now you have a working discord bot. Change up the code in `index.js` to add more functionality!

## Important Links
* [Discord.js Documentation](https://discord.js.org/#/docs)
* [Discord.js server](https://discord.gg/bRCvFy9) 
* [Discord API server](https://discord.gg/rV4BwdK)

## Help
I don't exactly intend on helping everyone with any problems they have with this. if there's a bug i'll fix it but support is only available to the friends that I actually gave a link to this project to, Sorry. Check the Discord.js server above for discord.js related help and Google for all the JavaScript related help needs.