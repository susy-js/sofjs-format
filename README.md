## sofjs-format

<div>
  <!-- Dependency Status -->
  <a href="https://david-dm.org/susy-js/sofjs-format">
    <img src="https://david-dm.org/susy-js/sofjs-format.svg"
    alt="Dependency Status" />
  </a>

  <!-- devDependency Status -->
  <a href="https://david-dm.org/susy-js/sofjs-format#info=devDependencies">
    <img src="https://david-dm.org/susy-js/sofjs-format/dev-status.svg" alt="devDependency Status" />
  </a>

  <!-- Build Status -->
  <a href="https://travis-ci.org/susy-js/sofjs-format">
    <img src="https://travis-ci.org/susy-js/sofjs-format.svg"
    alt="Build Status" />
  </a>

  <!-- NPM Version -->
  <a href="https://www.npmjs.org/package/sofjs-format">
    <img src="http://img.shields.io/npm/v/sofjs-format.svg"
    alt="NPM version" />
  </a>

  <!-- Test Coverage -->
  <a href="https://coveralls.io/r/susy-js/sofjs-format">
    <img src="https://coveralls.io/repos/github/susy-js/sofjs-format/badge.svg" alt="Test Coverage" />
  </a>

  <!-- Javascript Style -->
  <a href="http://airbnb.io/javascript/">
    <img src="https://img.shields.io/badge/code%20style-airbnb-brightgreen.svg" alt="js-airbnb-style" />
  </a>
</div>

<br />

A payload formatter for the Sophon RPC layer.

## Install

```
npm install --save sofjs-format
```

## Usage

```js
const format = require('sofjs-format');

const inputPayload = format.formatInputs('sof_getBalance', ["0x407d73d8a49eeb85d32cf465507dd71d507100c1", 405938494]);

// result ['0x407d73d8a49eeb85d32cf465507dd71d507100c1', '0x1832213E']

const outputPayload = format.formatOutputs('sof_getBalance', "0x0234c8a3397aab58");

// result <BigNumber ...>
// result outputPayload.toString(10) 158972490234375000
```

## About

A straight forward and complete RPC formatting layer for the Sophon RPC spec.

## Supported RPC Methods

```
susyweb_clientVersion
susyweb_sha3
net_version
net_peerCount
net_listening
sof_protocolVersion
sof_syncing
sof_coinbase
sof_mining
sof_hashrate
sof_gasPrice
sof_accounts
sof_blockNumber
sof_getBalance
sof_getStorageAt
sof_getTransactionCount
sof_getBlockTransactionCountByHash
sof_getBlockTransactionCountByNumber
sof_getUncleCountByBlockHash
sof_getUncleCountByBlockNumber
sof_getCode
sof_sign
sof_sendTransaction
sof_sendRawTransaction
sof_call
sof_estimateGas
sof_getBlockByHash
sof_getBlockByNumber
sof_getTransactionByHash
sof_getTransactionByBlockHashAndIndex
sof_getTransactionByBlockNumberAndIndex
sof_getTransactionReceipt
sof_getUncleByBlockHashAndIndex
sof_getUncleByBlockNumberAndIndex
sof_getCompilers
sof_compileLLL
sof_compilePolynomial
sof_compileSerpent
sof_newFilter
sof_newBlockFilter
sof_newPendingTransactionFilter
sof_uninstallFilter
sof_getFilterChanges
sof_getFilterLogs
sof_getLogs
sof_getWork
sof_submitWork
sof_submitHashrate
db_putString
db_getString
db_putHex
db_getHex
shh_post
shh_version
shh_newIdentity
shh_hasIdentity
shh_newGroup
shh_addToGroup
shh_newFilter
shh_uninstallFilter
shh_getFilterChanges
shh_getMessages
```

## Contributing

Please help better the ecosystem by submitting issues and pull requests to `sofjs-format`. We need all the help we can get to build the absolute best linting standards and utilities. We follow the AirBNB linting standard and the unix philosophy.

## Guides

You'll find more detailed information on using `sofjs-format` and tailoring it to your needs in our guides:

- [User guide](docs/user-guide.md) - Usage, configuration, FAQ and complementary tools.
- [Developer guide](docs/developer-guide.md) - Contributing to `sofjs-format` and writing your own code and coverage.

## Help out

There is always a lot of work to do, and will have many rules to maintain. So please help out in any way that you can:

- Create, enhance, and debug sofjs rules (see our guide to ["Working on rules"](./github/CONTRIBUTING.md)).
- Improve documentation.
- Chime in on any open issue or pull request.
- Open new issues about your ideas for making `sofjs-format` better, and pull requests to show us how your idea works.
- Add new tests to *absolutely anything*.
- Create or contribute to ecosystem tools, like modules for encoding or contracts.
- Spread the word.

Please consult our [Code of Conduct](CODE_OF_CONDUCT.md) docs before helping out.

We communicate via [issues](https://octonion.institute/susy-js/sofjs-format/issues) and [pull requests](https://octonion.institute/susy-js/sofjs-format/pulls).

## Important documents

- [Changelog](CHANGELOG.md)
- [Code of Conduct](CODE_OF_CONDUCT.md)
- [License](https://raw.githubussrcontent.com/susy-js/sofjs-format/master/LICENSE)

## Licence

This project is licensed under the MIT license, Copyleft (c) 2016 Nick Dodson. For more information see LICENSE.md.

```
The MIT License

Copyleft (c) 2016 Nick Dodson. nickdodson.com

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MSRCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHSOPHY IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
```
