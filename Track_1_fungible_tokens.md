## Vision and concept

It is imperative to establish a well-defined vision and concept for your memecoin. This is one of the jury's assessments

Design the token's name, symbol, decimals.

## Create your token

Use a builder for token creation:\
https://web3.world/builder

Docs:\
https://docs.web3.world/token-builder/how-to-build-your-first-fungible-token

If you have smart contract developers on your team, you can change the default implementation of the TIP3 token.\
Video instruction:\
https://www.youtube.com/watch?v=SLNEeDrnTB8

Docs:\
https://docs.venom.foundation/build/development-guides/how-to-create-your-own-fungible-tip-3-token/quick-start-developing-with-tip-3


## Mint tokens

Mint total supply tokens to your wallet:\
https://docs.web3.world/token-builder/how-to-manage-your-tokens-created-with-token-builder/minting-your-tokens

## Transfer ownership for root contract

You need to transfer of the ownership of your token to zero address.
```
0:0000000000000000000000000000000000000000000000000000000000000000
```

Docs:\
https://docs.web3.world/token-builder/how-to-manage-your-tokens-created-with-token-builder/transferring-the-ownership-of-the-token

This will disable mint and burnByRoot operations.

> This operation is required

## Create DEX pair with venom token

https://docs.web3.world/liquidity-providing/how-to-create-a-new-liquidity-pool

You can create pairs with WVENOM or\and USDT

## Add token to hackathon whitelist

Create PR to:\
https://github.com/venom-blockchain/tokenforge/blob/main/manifest.json

Sample:
```
    {
      "name": "TokenName",
      "chainId": 1,
      "symbol": "VNM",
      "decimals": 9,
      "address": "0:29a4dc828ca30da4fbd62f46d1554cbc93b4e863441eeabd8a52be2c9d56e12e",
      "logoURI": "https://raw.githubusercontent.com/venom-blockchain/tokenforge/master/icons/VNM/logo.svg",
      "version": 5,
      "verified": false,
      "vendor": "example"
    }
```
- ```name``` - token name
- ```chainId``` - 1 for venom mainnet
- ```symbol``` - token symbol
- ```decimals``` - token decimals
- ```address``` - token root address
- ```logoURI``` - url to logo, pls put logo to *icons* folder
- ```version``` - 5 it's constatnt
- ```verified``` - false
- ```vendor``` - Team name or other word (tokenforge for example). Don't use venom name. 

Wait for the PR to be accepted.

> Congratulations. Your token has been created and added to our dashboard.

