## SimpleStorage

### Deploy

```shell
$ forge script script/DeploySS.s.sol --rpc-url <your_rpc_url> --private-key <your_private_key>
```

### Cast

```shell
## To write the contract by interacting with the 'function store(uint256 _favoriteNumber)'
$ cast send <contractAddress> "store(uint256)" <numberToStore> --rpc-url <your_rpc_url> --private-key <your_private_key>

## To read the contract by interacting with 'function retrieve()' which will return a hex
$ cast call <contractAddress> "retrieve()" --rpc-url <your_rpc_url> --private-key <your_private_key>

## To convert the hex to decimal
$ cast --to-base <hex> dec
```

## Foundry

**Foundry is a blazing fast, portable and modular toolkit for Ethereum application development written in Rust.**

Foundry consists of:

- **Forge**: Ethereum testing framework (like Truffle, Hardhat and DappTools).
- **Cast**: Swiss army knife for interacting with EVM smart contracts, sending transactions and getting chain data.
- **Anvil**: Local Ethereum node, akin to Ganache, Hardhat Network.
- **Chisel**: Fast, utilitarian, and verbose solidity REPL.

## Documentation

https://book.getfoundry.sh/

## Usage

### Build

```shell
$ forge build
```

### Test

```shell
$ forge test
```

### Format

```shell
$ forge fmt
```

### Gas Snapshots

```shell
$ forge snapshot
```

### Anvil

```shell
$ anvil
```

### Deploy

```shell
$ forge script script/Counter.s.sol:CounterScript --rpc-url <your_rpc_url> --private-key <your_private_key>
```

### Cast

```shell
$ cast <subcommand>
```

### Help

```shell
$ forge --help
$ anvil --help
$ cast --help
```
