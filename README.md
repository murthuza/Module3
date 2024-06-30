
# MyTokenMs

MyTokenMs is a simple ERC-20-like token contract implemented in Solidity. This contract allows the owner to mint and burn tokens, as well as transfer tokens between addresses.

## Contract Details

- **Owner**: The owner of the contract, who has special privileges such as minting new tokens.
- **Token Name**: Murthuza
- **Token Symbol**: Ms
- **Total Supply**: The total number of tokens in circulation.

## Functions

### `constructor()`
The constructor function initializes the contract, setting the message sender as the owner and defining the token name and symbol. The total supply is initially set to zero.

### `mint(address _address, uint256 _value)`
Mints new tokens and assigns them to the specified address. Only the contract owner can mint new tokens.

- **Parameters:**
  - `_address`: The address to which the new tokens will be assigned. Must be the owner's address.
  - `_value`: The number of tokens to mint.

### `burn(address _address, uint256 _value)`
Burns the specified amount of tokens from the given address. This reduces both the total supply and the balance of the address.

- **Parameters:**
  - `_address`: The address from which tokens will be burned.
  - `_value`: The number of tokens to burn.

### `transfer(address _from, address _to, uint256 value)`
Transfers tokens from one address to another. This function can be called by anyone.

- **Parameters:**
  - `_from`: The address from which tokens will be transferred.
  - `_to`: The address to which tokens will be transferred.
  - `value`: The number of tokens to transfer.

## Modifiers

### `onlyOwner`
Ensures that the function can only be executed by the contract owner.

## Usage

To interact with the MyTokenMs contract, you can use any Ethereum development environment such as Remix, Truffle, or Hardhat. Deploy the contract and call the functions as needed.
