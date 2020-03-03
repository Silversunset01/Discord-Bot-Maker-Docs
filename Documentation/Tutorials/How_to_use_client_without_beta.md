## How to use `client` in non-beta

Since `client` isn't defined in non-beta, you must use `this.getDBM().Bot.bot` to call the Discord.js Client. However, `this.getDBM().Bot.bot` is too long to type and we don't want to do that, do we? To work around this, you can put the following code in a Run Script inside a Bot Initialization event.
```JavaScript
global.client = this.getDBM().Bot.bot
```
