# PUFFScoin dApp Wallet

The PUFFScoin wallet.

[![Build Status](https://travis-ci.org/puffscoin/meteor-dapp-wallet.svg?branch=master)](https://travis-ci.org/puffscoin/meteor-dapp-wallet)

**PLEASE NOTE:** This wallet is under development,
and may contain bugs! Please use at your own risk.

## Install

If you don't have [Meteor](https://www.meteor.com/install):

    $ curl https://install.meteor.com/ | sh

Install npm dependencies:

    $ cd meteor-dapp-wallet/app
    $ npm install

## Development

Start a `gpuffs` node:

    $ gpuffs --ws --wsorigins "http://localhost:3000" --unlock <your account>

Run dev server:

    $ cd meteor-dapp-wallet/app
    $ meteor

Navigate to http://localhost:3000

## Deployment

To create a build:

    $ npm install -g meteor-build-client
    $ cd meteor-dapp-wallet/app
    $ npm install
    $ meteor-build-client ../build --path ""

This will generate the files in the `../build` folder.

Navigating to `index.html` will start the app, but you will need to serve it over a local server like [MAMP](https://www.mamp.info).

---

## Gas usage statistics

- Deploy original wallet: 1 230 162
- Deploy wallet stub: 184 280
- Simple Wallet transaction: 64 280
- Multisig Wallet transaction below daily limit: 79 280
- Multisig Wallet transaction above daily limit: 171 096
- 1 Multisig confirmation: 48 363
