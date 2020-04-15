# Melif

Melif is an SDK that helps in the integration between the developer and the Mercado Libre API

## Installation

Use npm or yarn to perform the installation.

```bash
npm install melif
```
or 
```bash
yarn add melif
```

## Usage

First, you need to create an instance of melif with your information.
```javascript
var M = require('melif')

// Fill in the required information
const Melif = new M({
    api_root_url: 'https://api.mercadolibre.com',
    auth_url: 'https://auth.mercadolibre.com/authorization',
    oauth_url: 'https://api.mercadolibre.com/oauth/token',
    client_id: 'your mercado libre client_id',
    client_secret: 'your mercado libre client_secret',
});

module.exports = Melif;
```

Now just import your instance of Melif and use it!
```javascript
const Melif = require('./Melif');

// Now you can use all the methods of melif!
var auth_url = Melif.getAuthUrl("http://localhost:3000/v1/authentication/authorize");

console.log(auth_url)
```
## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

<!--Please make sure to update tests as appropriate-->

## License
[MIT](https://choosealicense.com/licenses/mit/)