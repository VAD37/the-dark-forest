# contract-design

There are lots of stuff in design gameplay have to do with the limitation of current contracts standard.
Below are just some of difficulty I might bump in.

- A master contract to control inflation token. Decide which player NFT buildings allowed to mint.
- The revenue model is wait for enough time to claim the resources from buildings.
- Player Resources should be ERC1155 token. No doubt.
- The main inflation rate is controlled by the master contract. It is constant storage through upgradeable proxy contract. Or game config contract.
- For player army, commander. It must be a factory/clone contract going through the logic of master contract. The owner have abilities to change URI as they wish. Only the unique name ID is stored on master.
- The logic for claiming rewards.
- How to apply data from the master contract to player proxy NFT.
