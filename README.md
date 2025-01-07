## What is Upgradable Contracts?

Upgradable contracts are smart contracts that can be modified after deployment to the blockchain. This flexibility is crucial for fixing bugs, adding features, or adapting to changing requirements without disrupting the continuity of existing contracts. Upgradable contracts typically involve a proxy pattern, where the logic is separated from the data. The proxy contract holds the data and delegates calls to a logic contract, which can be replaced with a new version while preserving the state in the proxy. This mechanism ensures that applications can evolve over time while maintaining the integrity and security of their operations.

## What is UUPS Proxy?

UUPS (Universal Upgradeable Proxy Standard) is a proxy pattern that allows the underlying logic of a contract to be upgraded without changing its address. It is a standard interface for proxy contracts that enables upgrading the implementation of a contract without interrupting the proxy's operation. The UUPS proxy pattern is widely used in the Ethereum ecosystem for building upgradable contracts.

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
