# Ampleforth

[![Build Status](https://travis-ci.com/ampleforth/uFragments.svg?token=xxNsLhLrTiyG3pc78i5v&branch=master)](https://travis-ci.com/ampleforth/uFragments)&nbsp;&nbsp;[![Coverage Status](https://coveralls.io/repos/github/frgprotocol/uFragments/badge.svg?branch=master&t=GiWi8p)](https://coveralls.io/github/frgprotocol/uFragments?branch=master)

Ampleforth (code name uFragments) is a decentralized elastic supply protocol. It maintains a stable unit price by adjusting supply directly to and from wallet holders. You can read the [whitepaper](https://drive.google.com/file/d/1I-NmSnQ6E7wY1nyouuf-GuDdJWNCnJWl/view) for the motivation and a complete description of the protocol.

This repository is a collection of [smart contracts](https://www.ampleforth.org/redbook/) that implement the Ampleforth protocol on the Ethereum blockchain.

The official contract addresses are:
- ERC-20 Token: [0xD46bA6D942050d489DBd938a2C909A5d5039A161](https://etherscan.io/token/0xd46ba6d942050d489dbd938a2c909a5d5039a161)
- Supply Policy: [0x1B228a749077b8e307C5856cE62Ef35d96Dca2ea](https://etherscan.io/address/0x1b228a749077b8e307c5856ce62ef35d96dca2ea#contracts)
- Orchestrator: [0x6fb00a180781e75f87e2b690af0196baa77c7e7c](https://etherscan.io/address/0x6fb00a180781e75f87e2b690af0196baa77c7e7c)
- Market Oracle: [0x99c9775e076fdf99388c029550155032ba2d8914](https://etherscan.io/address/0x99c9775e076fdf99388c029550155032ba2d8914)
- CPI Oracle: [0xa759f960dd59a1ad32c995ecabe802a0c35f244f](https://etherscan.io/address/0xa759f960dd59a1ad32c995ecabe802a0c35f244f)

## Table of Contents

- [Install](#install)
- [Testing](#testing)
- [Contribute](#contribute)
- [License](#license)


## Install

```bash
# Install project dependencies
npm install

# Install ethereum local blockchain(s) and associated dependencies
npx setup-local-chains
```

## Testing

``` bash
# You can use the following command to start a local blockchain instance
npx start-chain [ganacheUnitTest|gethUnitTest]

# Run all unit tests
npm test

# Run unit tests in isolation
npx truffle --network ganacheUnitTest test test/unit/uFragments.js
```

## Contribute

To report bugs within this package, create an issue in this repository.
For security issues, please contact dev-support@ampleforth.org.
When submitting code ensure that it is free of lint errors and has 100% test coverage.

``` bash
# Lint code
npm run lint

# View code coverage
npm run coverage
```

## License

[GNU General Public License v3.0 (c) 2018 Fragments, Inc.](./LICENSE)
