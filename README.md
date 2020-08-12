# valorant.js
## An API Wrapper for valorant with oauth support (now implemented)
### Warning: This lib is currently in development. Some bugs can occur!

## V1.0.5
In v1.0.5 Oauth has been added and is now available! For now you can only get the user's wallet.\
Don't worry, more is coming soon! Just come back here at a later date and check.

## Installation
```npm install valorant.js --save```

## Example 
<> = Replace with your value (remove <>)
```js
(async () => {
  try {

    const Valorant = require("valorant.js");
  
    const valorant = new Valorant.ValorantClient({
      username: "<YOUR_USERNAME>",
      password: "<YOUR_PASSWORD>",
      region: Valorant.Region.<YOUR_REGION(choose between: eu, na, ap)>
    });

    await valorant.login();
    const balance = await valorant.getWallet();
    console.log(balance);

  } catch(err) {
    console.error(err)
  }
})();
```

### Support
* [Discord](https://discord.gg/q37Dfyn)

### Credit
* [Sprayxe](https://twitter.com/Sprayxe_) `@Sprayxe#0742`
* [Speeedyyyy](https://twitter.com/Speeedyyyytv) `@Speeedyyyy#2367`
* [RumbleMike](https://twitter.com/RumbleMikee) `@RumbleMike#5406`

### Dependencies
* [Axios](https://www.npmjs.com/package/axios)
* [Colors](https://www.npmjs.com/package/colors)

