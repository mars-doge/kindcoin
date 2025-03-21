<div align="center">

![foxdemo](https://kindcoin.cc/git/img/kcGITicon.png) 

Kindcoin Core [KCCC, K] </div>
=====================================

https://kindcoin.cc

What is Kindcoin?
----------------

Kindcoin is a decentralised digital currency with near-instant transaction speeds and negligible transaction fees built upon Proof of Stake 3.0 (PoSV3, BPoS) as
introduced by the Blackcoin development team.

For more information about Kindcoin itself, see https://kindcoin.cc.

What is Kindcoin?
----------------

Kindcoin is the name of open source software which enables the use of this currency. It takes Kindcoin to the next level by building upon
Bitcoin Core 0.13.2 with some patches from newer Bitcoin Core versions to offer performance enhancements, wider compatibility with third party services and a more advanced base.

For more information, as well as an immediately useable, binary version of the Kindcoin software, see https://kindcoin.cc.

Ports
-----

P2P | RPC
------------ | -------------
21538 | 21537

License
-------

Kindcoin is released under the terms of the MIT license. See [COPYING](COPYING) for more
information or see https://opensource.org/licenses/MIT.

Development Process
-------------------

The `master` branch is regularly built and tested, but is not guaranteed to be
completely stable. [Tags](https://github.com/kindcoincore/kindcoin/tags) are created
regularly to indicate new official, stable release versions of Kindcoin.

Change log can be found in [CHANGELOG.md](CHANGELOG.md).

The contribution workflow is described in [CONTRIBUTING.md](CONTRIBUTING.md).


Testing
-------

Testing and code review might be the bottleneck for development. Please help out by testing
other people's pull requests, and remember this is a security-critical project where any mistake might cost people
lots of money.

### Automated Testing

Developers are strongly encouraged to write [unit tests](/doc/unit-tests.md) for new code, and to
submit new unit tests for old code. Unit tests can be compiled and run
(assuming they weren't disabled in configure) with: `make check`

There are also [regression and integration tests](/qa) of the RPC interface, written
in Python, that are run automatically on the build server.
These tests can be run (if the [test dependencies](/qa) are installed) with: `qa/pull-tester/rpc-tests.py`

The Travis CI system makes sure that every pull request is built for Windows, Linux, and OS X, and that unit/sanity tests are run automatically.

### Manual Quality Assurance (QA) Testing

Changes should be tested by somebody other than the developer who wrote the
code. This is especially important for large or high-risk changes. It is useful
to add a test plan to the pull request description if testing the changes is
not straightforward.
