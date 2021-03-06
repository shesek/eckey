0.4.0 / 2014-03-09
------------------
* Dropped sha256 and ripemd160 deps. Upgraded to crypto-hashing library.
* removed function wrapper
* Changed the way the constuctor works. Only supports input types of `Array`, `Buffer`, or `Uint8Array`. Does NOT randomly generate a private key anymore.
* added `publicKey` property
* ~~added `pubKeyHash`/`publicHash` property~~
* added `publicPoint`, removed `getPubPoint()`
* removed `getPub()`, use `publicKey` instead
* removed `getPubKeyHash()`, use `publicHash` or `pubKeyHash` instead
* removed `sign()` and `verify()`, methods can be accessed from [ecdsa](https://github.com/cryptocoinjs/ecdsa)
* added `privateExportKey` 
* removed `getExportedPrivateKey`, note that `getExportedPrivateKey` was essentially just a way to get WIF
* removed `decodeString()`, use package [coinstring][coinstring] in its place
* removed `getBitcoinAddress()`, use package [coinstring][coinstring] in its place
* removed `setCompressed`, use `compressed` property instead
* removed deps: `ecdsa`, `convert-hex`, `btc-address`, `bs58`
* updated deps: `ecurve` and `ecurve-names`
* removed `pubKeyHash` property, removes dependency upon `crypto-hashing`
* removed dep `crypto-hashing`

0.3.0 / 2014-02-03
------------------
* Removed bower and component support. Closes #8
* Upgraded version number so that `cryptocoin` could install. Changes in `0.2.1` could qualify for a `0.3.0`.

0.2.1 / 2014-01-23
------------------
* Update dependency package names/versions

0.2.0 / 2013-12-07
------------------
* added `recoverPubKey()` from package `ecdsa`
* updated to `ecdsa` `0.2.0`
* [remiq](https://github.com/remiq) fixed `getExportedPrivateKey()`, see: https://github.com/cryptocoinjs/eckey/pull/2
* updated name of deps: `bigi` and `bs58`

0.1.1 / 2013-12-05
------------------
* typo in `toString()` method. Closes #1

0.1.0 / 2013-11-20
------------------
* changed package name 
* removed AMD support

0.0.1 / 2013-11-12
------------------
* initial release

[coinstring]: https://github.com/cryptocoinjs/coinstring