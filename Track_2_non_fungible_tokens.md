# Required steps

## Vision and concept

It is imperative to establish a well-defined vision and concept for your NFT collection. This is one of the jury's assessments

## Create your NFT collection

Venom don't have UI builder for NFT. You need to use scripts for create and mint tokens.

### We recommend next properties for collection and NFT image for better display on the marketplace

**Collection**

For `preview` - we recommend: ratio 1:1, recommended dimensions 1000x1000px, jpeg, size less 200Kb. 
For `files`  - we recommend: 4:1 ratio, recommended dimensions 4000x1000px, jpeg.

**NFT**

For `preview` - we recommend: recommended dimensions 512x512, ratio 1:1, jpeg, size no more than 200Kb.
For `files` - as main file it may be pdf, docs, jpeg, gif, png, audio, video

**You can mint NFT collection from json file**

You can use deploy scripts from\  
https://github.com/blockchain-family/nft-marketplace-contracts.git

## Add NFT collection contract to whitelist

Create PR to:\
https://github.com/venom-blockchain/tokenforge/blob/main/nft-collections.json


Sample:
```
    {
      "address": "0:d000dfc3a575a0806958af3b6667f98e6acc19812c1249cdd64461da265eb279",
      "title": "Collection Title",
      "description": "Collection description",
      "preview": {
        "source": "https://link to image.png",
        "mimetype": "image/png"
      },
      "files": [
        {
          "source": ""https://link to image.png",
          "mimetype": "image/png"
        }
      ],
      "external_url": "yor site if you have"
    }
```
Wait for the PR to be accepted.

> Congratulations. Your NFT collection added to our dashboard.

# What next?

You can start promotion and selling NFT.
