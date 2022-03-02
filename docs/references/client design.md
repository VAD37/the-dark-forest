---
type: 
keywords: 
tags: 
foam_template:
  filepath: 'docs/references/client design.md' 
---

# client design

The time for #Hackathon is limited. A Text-based game is the best choice for the time being.

Current application is Unity Engine with Nethermind as the blockchain tools.

 The client will sent lots of transaction, so the game should not run WebGL and also I have no experience build web game. A window client with new wallet per client stored in plain text will be the solution for now. Player can send ETH to new account through rinkeby faucet.

## Features list

- Have the options to change URI endpoints for alchemy.
- Have GlobalChat available
- Have global event of people attacking, destroyed.
- Player can check their stats and inventory.
- Player can see other people in the world in a list.
- Player can attack other people in the world.
- Player have a nice overview of their civ.
- Have a list of last tx sending in popup notification that link to etherscan.
- UI and update balance of ETH and token.
- Show preview information of anyone being attacked.

## Gameplay features

- New civ name is unique. Same as ENS
- Player can use factory to create [[unit-archetype]]
- Can upgrade their [[building]]
- Calculate player army power.
- [[unit-archetype]] have background, image, unique name set by player.
- Can create [[commander]] with unique name and image asset through IPFS if possible.
- Player can edit their info, description, image, anthem, etc of their civ.
