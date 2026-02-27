# ETCswap V2 Periphery

Peripheral smart contracts for interacting with ETCswap V2 on Ethereum Classic — includes the Router for token swaps and liquidity management.

Forked from [Uniswap V2 Periphery](https://github.com/Uniswap/v2-periphery). The contracts are unmodified.

## Status: Reference Only

These contracts are deployed and immutable. This repo exists as a reference for the deployed bytecode. No further development is expected.

## Deployed Contracts

### Ethereum Classic (Chain ID: 61)

| Contract | Address |
|----------|---------|
| Router | [`0x79Bf07555C34e68C4Ae93642d1007D7f908d60F5`](https://etc.blockscout.com/address/0x79Bf07555C34e68C4Ae93642d1007D7f908d60F5) |
| Multicall | [`0x900cD941a2451471BC5760c3d69493Ac57aA9698`](https://etc.blockscout.com/address/0x900cD941a2451471BC5760c3d69493Ac57aA9698) |
| WETC | [`0x1953cab0E5bFa6D4a9BaD6E05fD46C1CC6527a5a`](https://etc.blockscout.com/token/0x1953cab0E5bFa6D4a9BaD6E05fD46C1CC6527a5a) |

### Mordor Testnet (Chain ID: 63)

| Contract | Address |
|----------|---------|
| Router | [`0x6d194227a9A1C11f144B35F96E6289c5602Da493`](https://etc-mordor.blockscout.com/address/0x6d194227a9A1C11f144B35F96E6289c5602Da493) |
| Multicall | [`0x41Fa0143ea4b4d91B41BF23d0A03ed3172725C4B`](https://etc-mordor.blockscout.com/address/0x41Fa0143ea4b4d91B41BF23d0A03ed3172725C4B) |
| WETC | [`0x1953cab0E5bFa6D4a9BaD6E05fD46C1CC6527a5a`](https://etc-mordor.blockscout.com/token/0x1953cab0E5bFa6D4a9BaD6E05fD46C1CC6527a5a) |

## Key Contracts

- **UniswapV2Router02.sol** — Swap and liquidity operations (addLiquidity, removeLiquidity, swapExact*)
- **UniswapV2Library.sol** — Helper functions for pair address calculation and price quoting
- **UniswapV2Migrator.sol** — Migration helper from V1 to V2

## Related Repos

- [v2-core](https://github.com/etcswap/v2-core) — Factory and Pair contracts
- [v2-interface](https://github.com/etcswap/v2-interface) — Trading frontend
- [sdks](https://github.com/etcswap/sdks) — TypeScript SDK monorepo

## Local Development

```bash
yarn install
yarn compile
yarn test
```

Solidity 0.6.6. Requires Node.js 10+.
