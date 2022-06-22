# Lotuscoins 

This is the ultra-stable backbone full node and wallet for lotuscoin,
the project aiming to be the longest lived and cheapest public blockchain.  

> openssl version
OpenSSL 1.1.0g  2 Nov 2017

If you have OpenSSL v. 1.0.x please use the "lotuscoin-openssl-1.0" version of this repository located here:  
http://github.com/Pamenarti/lotuscoin-openssl-1.0.git


--------------------------------------------

The Lotuscoin block chain is a log structured database.

The money supply is logarithmic.

The unit is log.

Dedicated to Log, Twig, Chip, Woody, and the rest of all y'all.  
 
--------------------------------------------

Technical Details:
```
* RPC Port = 9338

* P2P Ports = 8338 (testnet 18338)

* In Wallet mining/logging = Console, "setgenerate true"

* 120 Second Block Target, Diff Retarget every 1 hour

* 30 Confirms for spendable-coins

* Block reward = Harmonic Series

* 1000000/nHeight logs  (after first 100 blocks which form unspendable forest of 5187377 logs) 

* Money Supply = 1000000*(log(nHeight) + gamma)     gamma=Euler-Mascheroni constant 

* ECDSA curve: X9_62_prime256v1 

* Algo = Pure Skein (double skein) Bruce Schneier is a lumberjack and NSA didn't choose this algo.
```
Build Instructions

You will need these dependencies or equivalent:

--------------------------------------------
```
sudo apt-get install git build-essential libboost-all-dev libssl-dev qt-sdk libdb-dev libdb++-dev libminiupnpc-dev libqrencode-dev 
```

## Mining (lotuscutting)
--------------------------------------------

Get the source with this command:
```
git clone https://github.com/Pamenarti/lotuscoin.git
```
To build lotuscoin-qt issue “qmake” and then “make“.  qt4 is required, on some systems you may need to issue “export QT_SELECT=qt4” to ensure the proper version is used.

To build lotuscoind by itself navigate to /src/ and issue make -f makefile.unix.

--------------------------------------------
## Mining (lotuscutting)

To start lotuscutting with lotuscoind, simply launch it like this: 
```
```./lotuscoind setgenerate true```
```
For the graphical client, simply go into the debug window (under Help) and type:

```setgenerate true```

--------------------------------------------


## Changelog:

* v1.0 - Baruk Khazad!  lotuscutting for the masses.

* v1.1 - Hard fork to litecoin branch.  Block 3002.

* v1.2 - Solidifying full node w/ version update.  Block 962000

### Visit Lotuscoin.xyz for more information. 
