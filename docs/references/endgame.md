---
type: 
keywords: 
tags: 
foam_template:
  filepath: 'docs/references/endgame.md' 
---

# endgame

To finish the game. Destroy the master contract by overflow the balance of token.

```
    IERC20 token;
    function endgame() external {
        uint256 amount = token.balanceOf(msg.sender);
        uint256 balanceBeforeTransfer = token.balanceOf(address(this));
        // _transfer() function from ERC20 openzeppelin did not check for overflow.
        token.transferFrom(msg.sender, address(this), amount);
        uint256 balanceAfterTransfer = token.balanceOf(address(this));
        require(balanceAfterTransfer < balanceBeforeTransfer, "Game not overflow balance yet");
        selfdestruct(payable(address(this)));
    }
```
