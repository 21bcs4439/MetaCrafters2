# MetaCrafters2
This is a Solidity contract for a simple token called MyToken. It meets the following requirements:

It has public variables that store the details about the coin: name, abbreviation, and total supply.
It has a mapping of addresses to balances.
It has a mint function that takes an address and a value and increases the total supply and the sender's balance by that amount.
It has a burn function that takes an address and a value and decreases the total supply and the sender's balance by that amount, but only if the sender's balance is greater than or equal to the amount to be burned.
Usage

To use this contract, you would first deploy it to the Ethereum blockchain. Once it is deployed, you can call the mint() function to mint tokens for yourself or for other users. You can also call the burn() function to burn tokens from your own balance.

Example

The following example shows how to mint 100 tokens to the address 0x1234567890abcdef1234567890abcdef12345678.

MyToken token = new MyToken();
token.mint(0x1234567890abcdef1234567890abcdef12345678, 100);
The following example shows how to burn 50 tokens from your own balance.

MyToken token = new MyToken();
token.burn(msg.sender, 50);
Notes

This is a very simple token contract and does not include all of the features that a real-world token would need. For example, it does not support transfers between users.
It is important to note that burning tokens is a destructive operation and cannot be undone.
