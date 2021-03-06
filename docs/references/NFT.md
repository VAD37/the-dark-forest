---
type: 
keywords: 
tags: 
foam_template:
  filepath: 'docs/references/NFT.md' 
---

# NFT

As in [EIP-721](https://eips.ethereum.org/EIPS/eip-721)

```
NFTs can represent ownership over digital or physical assets. We considered a diverse universe of assets, and we know you will dream up many more:

    Physical property — houses, unique artwork
    Virtual collectables — unique pictures of kittens, collectable cards
    “Negative value” assets — loans, burdens and other responsibilities

NFTs are **distinguishable** and you must track the ownership of each one separately.
```

## State of NFTs

If you look at Verified contract on etherscan. You will see 19/20 contracts are NFTs.
Some have very good marketing practice and can easily reach 200-1000 holders in first day. Each of these success NFTs have their own unique image and gain around 20-60ETH per project.

The strategy was pretty simple, limited pre-render cool image on IPFS and then use it as fixed-URI for token. User mint new NFT without knowing the image. Some better project use actual random program async-event before sent to IPFS.

## The problems

As the original crypto kitties, the token does not hold baseURI of single image but multiple characteristics that can be used to generate same images again. But the most of the new NFTs project gone cheap and does not use this, this is not wrong or bad, it simply make the NFTs easy become worthless because everyone can make the same NFT, same image. Without pure marketing value or trust value of central authority, this model simply not sustainable for the future.

To address this, the project use try to give player attachment value and practical use for their NFTs token. Just so as long the game run, the token never lost value.

Check [[attachment-value]] for more details.

