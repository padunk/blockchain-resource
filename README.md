# My Resources learning Blockchain


## Tools
- [Metamask](https://metamask.io/)
- [Truffle](https://www.trufflesuite.com/truffle)
- [Ganache](https://www.trufflesuite.com/ganache)
- [Remix](https://remix.ethereum.org/#optimize=false&evmVersion=null)
- [Solidity compiler](https://www.npmjs.com/package/solc)


## Articles
- [5 tools](https://kingslanduniversity.com/5-must-have-tools-for-blockchain-developers/)
- [Ethereum Development Part 1](https://medium.com/hackernoon/ethereum-development-walkthrough-part-1-smart-contracts-b3979e6e573e)
- [Ethereum Development Part 2](https://hackernoon.com/ethereum-development-walkthrough-part-2-truffle-ganache-geth-and-mist-8d6320e12269)
- [Ethereum Development Part 3](https://hackernoon.com/ethereum-development-walkthrough-part-3-security-limitations-and-considerations-d482f05278b4)
- [Ethereum Development Part 4](https://hackernoon.com/ethereum-development-walkthrough-part-4-tokens-and-ercs-68645cf2f73e)
- [Ethereum Development Part 5](https://hackernoon.com/ethereum-development-walkthrough-part-5-making-a-dapp-4c2a3bbcd5e5)
- [List of Ethereum Tools](https://media.consensys.net/an-definitive-list-of-ethereum-developer-tools-2159ce865974)


## Youtube
- [Understanding the Blockchain Protocol](https://www.youtube.com/watch?v=gjwr-7PgpN8)
- [How does bitcoin actually work?](https://www.youtube.com/watch?v=bBC-nXj3Ng4&vl=en)


## Github
- [Tools List](https://github.com/ConsenSys/ethereum-developer-tools-list)


## Summary


### What is Gas
- Fee per computational step
- To avoid attack on program that run forever
- Solution to halting problem
- Fee also applied to operations that take up storage


### Gas Limit
- default: 3141592
- target: 150% of long-term EMA of gas usage
- counterpart to the block size limit in bitcoin


### Transactions
- nonce (anti-replay-attack)
- gasprice (amount of ether per unit gas)
- startgas (maximum gas consumable)
- to (destination address)
- value (amount of ETH to send)
- data (readable by contract code)
- v, r, s (ECDSA signature values)


### Receipts
- Every transaction have a receipts
- intermediate state root
- cumulative gas used
- logs: special feat in eth


### Logs
- append only, not readable by contracts
- -10x cheaper than storage
- up to 4 topics (32 bytes), plus data


### ABI (Application Binary Interface)
- Function calls are compiled into transaction data
- First 4 bytes: function ID
- next 32 bytes: first argument
- next 32 bytes: second argument


### World State
- Mapping between `addresses` and `account states`
- Included in `accaount states`: nonce, balance, storageRoot, codehash
