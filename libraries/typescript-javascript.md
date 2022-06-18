# TypeScript/JavaScript

### Install

```diff
npm install vipercord

or

npm install vipercord@latest
```

***

### Usage

```js
const { ViperClient } = require("vipercord");

const viper = new ViperClient({
    auth: "Api key",
    botID: "Bot id"
});

viper.post(SERVER_COUNT, SHARD_COUNT);
viper.log("Some Log Text so you know it Worked");
```

***

### Example

```js
const { ViperClient } = require("vipercord");

const viper = new ViperClient({
    auth: "AUTH_TOKEN", 
    botID: "819050202508890419"
});

viper.post(client.guilds.cache.size, 0).catch((err) => {
   viper.viperLogs(`Posting Stats has failed | Error: ${err}`);
});

viper.viperLogs("Posted Stats Successfully");
```

***
