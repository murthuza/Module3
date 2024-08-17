Murthuza Token Contract
This repository contains the Murthuza ERC20 token contract. The Murthuza token (symbol: Ms) is an ERC20 token built using the OpenZeppelin library. The contract owner, referred to as the "owner", has the ability to mint new tokens. Token holders can also burn their own tokens and transfer tokens to other addresses.

Features
Minting: The contract owner can mint new tokens.
Burning: Token holders can burn their own tokens.
Transferring: Token holders can transfer tokens to other addresses.
Contract Details
Name: Murthuza
Symbol: Ms
Functions
mintToken(address account, uint256 amount)
Mints new tokens and assigns them to the specified account. Only the contract owner can perform this action.

Parameters:

account: The address to receive the minted tokens.
amount: The number of tokens to mint.
burnToken(address account, uint256 amount)
Burns a specified amount of tokens from the caller's account.

Parameters:

account: The address from which tokens will be burned. Must be the caller's own address.
amount: The number of tokens to burn.
transferToken(address recipient, uint256 amount)
Transfers tokens from the caller's account to the specified recipient.

Parameters:

recipient: The address to receive the tokens.
amount: The number of tokens to transfer.
Modifiers
onlyowner
Ensures that only the contract owner can call the modified function.

Deployment
To deploy the Murthuza contract:

Ensure you have the required dependencies:

