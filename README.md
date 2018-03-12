Saros a crypto currency coin based on Neoscrypt alogrithm. Install right from the git repo, instructions are provided in doc/Install.md. If you still need help to install wallet daemon or configure it to setup with your mining pool you can get paid server via here https://github.com/goodthebest

Specifications
--------------

Name: SAROS
Ticker: SAROS
Mining algorithm: X11
Max Supply: 22M (2050 year)
Block Time: 60s
Premine: 5%
Reward halving: 25% per year

Masternode:
Masternode Collateral: 1500 SAROS
Masternode Reward: 50%
Block Reward = 10 SAROS 
Tx Fee = 0.001
Mainnet
-P2P Port: 9891
-RPC Port: 8992
addnode=207.246.71.251
addnode=45.77.64.146
addnode=45.77.64.146
addnode=207.246.71.251



Saros Core staging tree 0.12.1
===============================

`master:` [![Build Status](https://travis-ci.org/sarospay/saros.svg?branch=master)](https://travis-ci.org/sarospay/saros) `v0.12.0.x:` [![Build Status](https://travis-ci.org/sarospay/saros.svg?branch=v0.12.0.x)](https://travis-ci.org/sarospay/saros/branches) `v0.12.1.x:` [![Build Status](https://travis-ci.org/sarospay/saros.svg?branch=v0.12.1.x)](https://travis-ci.org/sarospay/saros/branches)

https://www.saros.org


What is Saros?
----------------

Saros is an experimental new digital currency that enables anonymous, instant
payments to anyone, anywhere in the world. Saros uses peer-to-peer technology
to operate with no central authority: managing transactions and issuing money
are carried out collectively by the network. Saros Core is the name of the open
source software which enables the use of this currency.

For more information, as well as an immediately useable, binary version of
the Saros Core software, see https://www.saros.org/get-saros/.


License
-------

Saros Core is released under the terms of the MIT license. See [COPYING](COPYING) for more
information or see https://opensource.org/licenses/MIT.

Development Process
-------------------

The `master` branch is meant to be stable. Development is normally done in separate branches.
[Tags](https://github.com/sarospay/saros/tags) are created to indicate new official,
stable release versions of Saros Core.

The contribution workflow is described in [CONTRIBUTING.md](CONTRIBUTING.md).

Testing
-------

Testing and code review is the bottleneck for development; we get more pull
requests than we can review and test on short notice. Please be patient and help out by testing
other people's pull requests, and remember this is a security-critical project where any mistake might cost people
lots of money.

### Automated Testing

Developers are strongly encouraged to write [unit tests](/doc/unit-tests.md) for new code, and to
submit new unit tests for old code. Unit tests can be compiled and run
(assuming they weren't disabled in configure) with: `make check`

There are also [regression and integration tests](/qa) of the RPC interface, written
in Python, that are run automatically on the build server.
These tests can be run (if the [test dependencies](/qa) are installed) with: `qa/pull-tester/rpc-tests.py`

The Travis CI system makes sure that every pull request is built for Windows
and Linux, OS X, and that unit and sanity tests are automatically run.

### Manual Quality Assurance (QA) Testing

Changes should be tested by somebody other than the developer who wrote the
code. This is especially important for large or high-risk changes. It is useful
to add a test plan to the pull request description if testing the changes is
not straightforward.

Translations
------------

Changes to translations as well as new translations can be submitted to
[Saros Core's Transifex page](https://www.transifex.com/projects/p/saros/).

Translations are periodically pulled from Transifex and merged into the git repository. See the
[translation process](doc/translation_process.md) for details on how this works.

**Important**: We do not accept translation changes as GitHub pull requests because the next
pull from Transifex would automatically overwrite them again.

Translators should also follow the [forum](https://www.saros.org/forum/topic/saros-worldwide-collaboration.88/).
