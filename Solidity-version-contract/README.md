# Documentation on how to run the project

## Contract introduction
- DaoFactory: Users can create their own DAO through factory contracts,displays a list of dao information,It's a collection of all the contracts.
- Authority: Used to manage permissions between accounts or contracts, which can be changed by proposal.
- DaoBaseInfo: It is used to save the basic information and types of dao.
- DaoManage: The dao's main logical management contract can manage funds or change contract parameters or contract permissions by requesting proposals.
- DaoMembers: Management contract for DAO members.
- ERC20Factory: This contract allows you to create your own ERC20 tokens.
- RouteManage: Routing contracts, record the addresses of all contracts.
- Vault: Token management contracts manage the expenditure and income of various tokens.
- Vote: The ability to initiate proposals for voting is the primary way to manage dao functionality.
## Dependencies

- Linux or Mac
- node ≥ 14

## Network & Contract
- Network Name: Avalanche FUJI C-Chain
- RPC URL: https://api.avax-test.network/ext/bc/C/rpc

### contract address

#### DaoFactory
0x0Fd9968e36523466a9C9A38D2581Fe0E199F8161
#### Authority
0x391A2bbDb62625cb0b9b4b6fAB5eB9647bB970Cd
#### DaoBaseInfo
0xb65daA181D320Eae638C8e71087e7e7C5c00db1b
#### DaoManage
0xF0b4F15495AE189A1F9e1210861aD47f18aD188f
#### ERC20Factory
0xCdd27850AC3f1D999166E11408DEA1137b28C5b7
#### RouteManage
0xb53E020F21bC17479443d7552F5681538d9De61c
#### Vault
0xDEf7188Bd888e230E7258410EF8a4e6Bee8AaaFF
#### Vote
0xe1240c60f37ae1CdeC036591C9814c1Fce8d986c

## Installing

```bash
git clone https://github.com/RainbowDAO/RainbowDAO-Protocol-Solidity-Avalanche-Hackathon.git
npm install
```

**Note**: Only the Metamask wallet is available for this demo


## Deploy Contracts
Open a local node or complete the information in the ```truffle-config.js``` and add the mnemonic to the ```secret```

```bash
npm install -g @truffle/hdwallet-provider
truffle compile && truffle migrate
```
You will deploy contracts
- DaoFactory

## Create a DAO
The creatDao in the DaoMain contract creates a DAO of its own, defining names, logos, and symbols

```creatDaoWithNewToken()``` or ```creatDao()```



