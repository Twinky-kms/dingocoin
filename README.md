# Dingocoin Core [DINGO, Ð]

![Dingocoin](https://dingocoin.com/img/logos/dingocoin/logo/dingo_coin256.png)

[![Build Status](https://travis-ci.com/dingocoin/dingocoin.svg?branch=master)](https://travis-ci.com/dingocoin/dingocoin)

Dingocoin is a cryptocurrency like Bitcoin, although it does not use SHA256 as
its proof of work (POW). Taking development cues from Tenebrix and Litecoin,
Dingocoin currently employs a simplified variant of scrypt.
- **Website:** [dingocoin.com](https://dingocoin.com)

## License – Much license ⚖️
Dingocoin Core is released under the terms of the MIT license. See
[COPYING](COPYING) for more information or see
<!-- [opensource.org](https://opensource.org/licenses/MIT)
<h1 align="center">
<img src="https://static.tumblr.com/ppdj5y9/Ae9mxmxtp/300coin.png" alt="Dingocoin" width="300"/>
<br/><br/>
Dingocoin Core [DOGE, Ð]  
</h1>

<div align="center">

[![DingocoinBadge](https://img.shields.io/badge/Doge-Coin-yellow.svg)](https://dingocoin.com)
[![MuchWow](https://img.shields.io/badge/Much-Wow-yellow.svg)](https://dingocoin.com)

</div> -->

Select language: EN | [CN](./README_zh_CN.md) | [PT](./README_pt_BR.md) | [FA](./README_fa_IR.md) | [VI](./README_vi_VN.md)

Dingocoin is a community-driven cryptocurrency that was inspired by a Shiba Inu meme. The Dingocoin Core software allows anyone to operate a node in the Dingocoin blockchain networks and uses the Scrypt hashing method for Proof of Work. It is adapted from Bitcoin Core and other cryptocurrencies.

For information about the default fees used on the Dingocoin network, please
refer to the [fee recommendation](doc/fee-recommendation.md).

**Website:** [dingocoin.com](https://dingocoin.com)

## Usage 💻

To start your journey with Dingocoin Core, see the [installation guide](INSTALL.md) and the [getting started](doc/getting-started.md) tutorial.

The JSON-RPC API provided by Dingocoin Core is self-documenting and can be browsed with `dingocoin-cli help`, while detailed information for each command can be viewed with `dingocoin-cli help <command>`. Alternatively, see the [Bitcoin Core documentation](https://developer.bitcoin.org/reference/rpc/) - which implement a similar protocol - to get a browsable version.

### Such ports

Dingocoin Core by default uses port `22556` for peer-to-peer communication that
is needed to synchronize the "mainnet" blockchain and stay informed of new
transactions and blocks. Additionally, a JSONRPC port can be opened, which
defaults to port `22555` for mainnet nodes. It is strongly recommended to not
expose RPC ports to the public internet.

| Function | mainnet | testnet | regtest |
| :------- | ------: | ------: | ------: |
| P2P      |   22556 |   44556 |   18444 |
| RPC      |   22555 |   44555 |   18332 |

## Ongoing development - Moon plan 🌒

Dingocoin Core is an open source and community driven software. The development
process is open and publicly visible; anyone can see, discuss and work on the
software.

Main development resources:

* [GitHub Projects](https://github.com/dingocoin/dingocoin/projects) is used to
  follow planned and in-progress work for upcoming releases.
* [GitHub Discussion](https://github.com/dingocoin/dingocoin/discussions) is used
  to discuss features, planned and unplanned, related to both the development of
  the Dingocoin Core software, the underlying protocols and the DOGE asset.  
* [Dingocoindev subreddit](https://www.reddit.com/r/dingocoindev/)

### Version strategy
Version numbers are following ```major.minor.patch``` semantics.

### Branches
There are 3 types of branches in this repository:

- **master:** Stable, contains the latest version of the latest *major.minor* release.
- **maintenance:** Stable, contains the latest version of previous releases, which are still under active maintenance. Format: ```<version>-maint```
- **development:** Unstable, contains new code for planned releases. Format: ```<version>-dev```

*Master and maintenance branches are exclusively mutable by release. Planned*
*releases will always have a development branch and pull requests should be*
*submitted against those. Maintenance branches are there for **bug fixes only,***
*please submit new features against the development branch with the highest version.*

## Contributing 🤝

If you find a bug or experience issues with this software, please report it
using the [issue system](https://github.com/dingocoin/dingocoin/issues/new?assignees=&labels=bug&template=bug_report.md&title=%5Bbug%5D+).

Please see [the contribution guide](CONTRIBUTING.md) to see how you can
participate in the development of Dingocoin Core. There are often
[topics seeking help](https://github.com/dingocoin/dingocoin/labels/help%20wanted)
where your contributions will have high impact and get very appreciation. wow.

## Communities 🚀🍾

You can join the communities on different social media.
To see what's going on, meet people & discuss, find the latest meme, learn
about Dingocoin, give or ask for help, to share your project.

Here are some places to visit:

* [Dingocoin subreddit](https://www.reddit.com/r/dingocoin/)
* [Discord](https://discord.gg/dingocoin)
* [Dingocoin Twitter](https://twitter.com/dingocoin)

## Very Much Frequently Asked Questions ❓

### How much dingo can exist? – So many puppies! 🐕
Mid 2022 (approximately a year and a half after release) there will be
approximately 100,000,000,000 coins.
Each subsequent block will grant 10,000 coins to encourage miners to continue to
secure the network and make up for lost wallets on hard drives/phones/lost
encryption passwords/etc.


### Such mining information ⛏

Dingocoin uses a simplified variant of the scrypt key derivation function as its
proof of work with a target time of one minute per block and difficulty
readjustment after every block. The block rewards are fixed and halve every
100,000 blocks. Starting with the 600,000th block, a permanent reward of
10,000 Dingocoin per block will be issued.  

Originally, a different payout scheme was envisioned with block rewards being
determined by taking the maximum reward as per the block schedule and applying
the result of a Mersenne Twister pseudo-random number generator to arrive at a
number between 0 and the maximum reward.

This was changed starting with block 5,000, to prevent large pools from gaming
the system and mining only high reward blocks. At the same time, the difficulty
retargeting was also changed from four hours to once per block (every minute),
implementing an algorithm courtesy of the DigiByte Coin development team, to
lessen the impact of sudden increases and decreases of network hashing rate.

**The current block reward schedule:**

1–4,999: 0–1,000,000 Dingocoin

5,000–99,999: 500,000 Dingocoin

100,000–199,999: 250,000 Dingocoin

200,000–299,999: 125,000 Dingocoin

300,000–399,999: 62,500 Dingocoin

400,000–499,999: 31,250 Dingocoin

500,000–599,999: 15,625 Dingocoin

600,000+: 10,000 Dingocoin

**The original block reward schedule, with one-minute block targets and four-hour difficulty readjustment:**

1–99,999: 0–1,000,000 Dingocoin

100,000–199,999: 0–500,000 Dingocoin

200,000–299,999: 0–250,000 Dingocoin

300,000–399,999: 0–125,000 Dingocoin

400,000–499,999: 0–62,500 Dingocoin

500,000–599,999: 0–31,250 Dingocoin

600,000+: 10,000 Dingocoin

### Wow plz make dingocoind/dingocoin-cli/dingocoin-qt

  The following are developer notes on how to build Dingocoin on your native platform. They are not complete guides, but include notes on the necessary libraries, compile flags, etc.

  - [OSX Build Notes](doc/build-osx.md)
  - [Unix Build Notes](doc/build-unix.md)
  - [Windows Build Notes](doc/build-windows.md)

### Such ports

- RPC 34646
- P2P 33117

## Development tips and tricks

**compiling for debugging**

Run `configure` with the `--enable-debug` option, then `make`. Or run `configure` with
`CXXFLAGS="-g -ggdb -O0"` or whatever debug flags you need.

**debug.log**

If the code is behaving strangely, take a look in the debug.log file in the data directory;
error and debugging messages are written there.

The `-debug=...` command-line option controls debugging; running with just `-debug` will turn
on all categories (and give you a very large debug.log file).

The Qt code routes `qDebug()` output to debug.log under category "qt": run with `-debug=qt`
to see it.

**testnet and regtest modes**

Run with the `-testnet` option to run with "play dingocoins" on the test network, if you
are testing multi-machine code that needs to operate across the internet.

If you are testing something that can run on one machine, run with the `-regtest` option.
In regression test mode, blocks can be created on-demand; see qa/rpc-tests/ for tests
that run in `-regtest` mode.

**DEBUG_LOCKORDER**

Dingocoin Core is a multithreaded application, and deadlocks or other multithreading bugs
can be very difficult to track down. Compiling with `-DDEBUG_LOCKORDER` (`configure
CXXFLAGS="-DDEBUG_LOCKORDER -g"`) inserts run-time checks to keep track of which locks
are held, and adds warnings to the debug.log file if inconsistencies are detected.
