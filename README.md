# 🐀 rat facts

![Image of rat emoji](https://github.com/RileyAbr/rat-facts-Discord-Bot/blob/master/rat_logo.png)

Rat facts is a Discord bot that delivers rat content.

## Features

-   Gives random facts about rats (over 100!)
-   Shows off pictures of rats
-   Tells jokes about rats
-   Consults the O-rat-cle to predict your future
-   Describes the lore beyond a great rat civil war

### Available Commands:

All commands are evoked with `!rat`.

-   `!rat fact (!rat)`
-   `!rat pic`
-   `!rat joke`
-   `!rat 8ball {question}`
-   `!rat lore`
-   `!rat help`
-   `!rat misc`

## Adding rat facts to a server

[Click here to invite rat facts to your server](https://discord.com/api/oauth2/authorize?client_id=717512371312132188&permissions=130048&scope=bot)

## Technical Details

Rat facts is built as a Node.js project. It relies heavily on the [Discord.js](https://discord.js.org/#/) module to make working with Discord's API much easier. Much of the information used for the various commands are stored in local JSON files, making them easy to expand with additional facts, jokes, or photos. The bot is hosted on a Heroku instance with a single worker Dyno calling the node project to start.

### Expanding the Bot

If you would like to develop on the bot yourself, simply clone the repo and provide your own credentials. The main file (`rat.js`) reads from a configuration file (`config.json`) for a `CONFIG_BOT_TOKEN` and `DEV_BOT_TOKEN`. These will match the bot token generated by Discord when you register the app via the Discord Developer Portal. Fill in your own token (only the `CONFIG_BOT_TOKEN` is necessary) and run `npm start` to start the bot **NOTE:** your new bot must be added to your server; the invite link can be generated within the Discord Developer Portal.
