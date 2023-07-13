# Metacrafters-Solidity
The assessment demonstrates how mint, burn, and totalSupply function in NFT Token. The purpose of this program is to provide people with basic knowledge.
# Description
Solidity is an object-oriented programming language used to build smart contracts on multiple blockchain systems, the most prominent of which being Ethereum.
# Getting Started
To run this code go to https://remix.ethereum.org/ Create a new file (example MyToken.sol) and paste the code below.
contract MyToken {

// public variables here
string public tokenName = "Saba"; string public tokenAbbrv = "SB"; uint public totalSupply = 0; // mapping variable here mapping (address => uint) public balances; // mint function function mint (address _address, uint _value) public { totalSupply += _value; balances [_address] += _value; } // burn function function burn (address _address, uint _value) public { if (balances[_address]>=_value){ totalSupply -= _value; balances [_address] -= _value; }

} }
# Author
Saba, Patricia Anne G. Email: 8215066@ntc.edu.ph
