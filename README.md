# Phala ERC20

The contract has been deployed at [0x6c5ba91642f10282b576d91922ae6448c9d52f4e](https://etherscan.io/address/0x6c5ba91642f10282b576d91922ae6448c9d52f4e).

## Install dependencies

Prefer node.js v12.16.2

```bash
yarn
```

## Deploy

```bash
truffle migrate --network mainnet
```

## Verify on Etherscan

```bash
truffle run verify PHAToken --network mainnet
```

## Approve MultiSend.co

```bash
truffle console --network mainnet
```

Then in the console:

```js
pha = await PHAToken.deployed()
UNIT = new web3.utils.BN('1000000000000000000')
await pha.approve('0x1E860B41498BFFbe50106114b55c0E76Ff02c559', UNIT.muln(10000))
```
