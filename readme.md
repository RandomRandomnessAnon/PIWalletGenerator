# PIWalletGenerator

PIWalletGenerator is for generating a new PI seed and Public/Secret key pair and creating it on the PI Network.

Three seperate scripts:

DecodeWallet.js - Inputs your existing PI Wallet's 12-word mneomic and returns it's public/secret key pair

WalletKeyGen.js - generates a 12-work mnemonic as well as public/secret key pair

CreateWalletOnPiNetwork.js - Using an existing secret corresponding to an existing account on the PI Network, you are able to create the new wallet whose keys were created in WalleteyGen.js

## Requirements/installation
NodeJS/NPM - download from https://nodejs.org/en/download
Package Dependencies (run in your woring directory where you cloned)
```bash
npm install stellar-sdk @hawkingnetwork/ed25519-hd-key-rn bip39 readline
```

## Usage

```javascript
node DecodeWallet.js
//inputs your existing PI Wallet's 12-word mneomic and returns it's public/secret key pair
```

```javascript
node WalletKeyGen.js
//generates a 12-work mnemonic as well as public/secret key pair
```

```javascript
node CreateWalletOnPiNetwork.js
//First input is a secret key corresponding to a wallet that already exists on the PI network
//Second input is the newly created secret key from WalletKeyGen.js
```

## Contributing

Pull requests are welcome

## License

[MIT](https://choosealicense.com/licenses/mit/)