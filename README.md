# Track Crypto Currency

Tracking software for almost any crypto currency

<img src="https://bitcoin.org/img/icons/opengraph.png" width="100">
<img src="http://files.coinmarketcap.com.s3-website-us-east-1.amazonaws.com/static/img/coins/200x200/litecoin.png" width="100">
<img src="http://files.coinmarketcap.com.s3-website-us-east-1.amazonaws.com/static/img/coins/200x200/monero.png" width="100">
<img src="http://files.coinmarketcap.com.s3-website-us-east-1.amazonaws.com/static/img/coins/200x200/ethereum.png" width="100">
<img src="http://xospiritus.com/wp-content/uploads/2013/11/and-many-more-JPEG.jpg" width="100">

Works on **Mac, Ubuntu and Windows**

<img src="https://i.gadgets360cdn.com/large/bitcoin_chip_pixabay_1495081418418.jpg?output-quality=80" width="800">

## Install

#### Mac OS

Install:

```
git clone https://github.com/pendmining/pendtracking
```

#### Windows

Before your start, make sure you have Putty(https://www.putty.org/) installed or use a console emulator like CMDER(http://cmder.net/):

Install:

```
git clone https://github.com/pendmining/pendtracking
```

#### Ubuntu

Install

```
git clone https://github.com/pendmining/pendtracking
```

#### Usage

Cd into directory

```
cd pendtracking
```

Depending on your operating system you should use

```
./cli-mac -> Mac OS
sudo ./cli-linux -> Ubuntu
./cli-win.exe -> Windows
```

###### Track addresses

Example 1 - Check balance:

```
./cli-mac --cur btc --balance 1F1tAaz5x1HUXrCNLbtMDqcw6o5GNn4xqX
```

Returns:

```
(2.49640000 BTC)
```

Example 2 - Basic track:

```
./cli-mac --cur btc --track 1F1tAaz5x1HUXrCNLbtMDqcw6o5GNn4xqX
```

Returns:

```
1F1tAaz5x1HUXrCNLbtMDqcw6o5GNn4xqX => 1NnJT38274MT5bqbrzEfSThEwdaRuvx2dG (0.00324534 BTC)
                                      3EcWc71mpU2RGyyHdRSXeckh37Kh4uuDJy (0.52464000 BTC)
                                      19KRB1BaiotszRiqWX19yuCqSgLrJWKjPq (2.65540000 BTC)
                                      1HB8qtAoSsowZ1SR6dAfB8or5tuXPWusKm (0.95020350 BTC)
```

Example 3 - Advanced track, specify level:

```
./cli-mac --cur btc --track 1F1tAaz5x1HUXrCNLbtMDqcw6o5GNn4xqX --level 2
```

Returns:

```
1F1tAaz5x1HUXrCNLbtMDqcw6o5GNn4xqX => 1NnJT38274MT5bqbrzEfSThEwdaRuvx2dG (0.45724000 BTC) => 1NDyJtNTjmwk5xPNhjgAMu4HDHigtobu1s (0.07564456 BTC)
                                                                                             1HDj2ruV5Wts42dUcQn45A1FvMQmUoZhyQ (0.02345460 BTC)

                                      1BcWc71mpU2RGyyHdRSXeckh37Kh4uuDJy (0.98900000 BTC) => 3L5bbRAsKW59itMrZirgj8btexnz7Zdcyr (0.00142445 BTC)

                                      19KRB1BaiotszRiqWX19yuCqSgLrJWKjPq (0.04718480 BTC) => 151jXCCsxFh1k9bmrRLAeQutBUf1PAu21X (0.00014500 BTC)
                                                                                             1L5bbRAsKW59itMrZirgj8btexnz7Zdcyr (2.14514565 BTC)
                                                                                             1QjLTHs1agc46G21jRaEe7uGhiiR6U8fat (0.461514550 BTC)

                                      1HB8qtAoSsowZ1SR6dAfB8or5tuXPWusKm (0.00958471 BTC) => 1Em7pxEVJNCKfE8TojCGU5TY5icxFhAbJK (0.001451461 BTC)
```

###### Check if two addresses are related

```
./cli-mac --cur btc --compare address_1 address_2
```

Returns:

```
True or False
```

**Just in cases you can not execute the file:**

```
chmod +x cli-mac - Mac OS
chmod +x cli-linux -> Linux
chmod +x cli-win -> Windows
```

## Currency List

```
--cur btc -> Bitcoin
--cur ltc -> Litecoin
--cur dash -> Dash
--cur xmr -> Monero
--cur zec -> ZCash
--cur bch -> Bitcoin Cash
--cur eth -> Ethereum
--cur xzc -> ZCoin
--cur decred -> Decred
--cur neo -> Neo
--cur qtum -> Qtum
--cur btcd -> Bitcoin Dark
--cur bcn -> Bytecoin
--cur doge -> DogeCoin
--cur xrp -> Ripple
--cur xvg -> Verge
--cur xlm -> Stellar
--cur zen -> ZENCash
--cur ant -> Aragon
--cur blk -> BlackCoin
--cur cvc -> Civic
--cur rep -> Augur
```

## Coming soon

Support for more crypto currencies will be added regularly.<br />
In addition to that we will add more advanced strategies like tree structures for displaying the history with timestamps.

## Engineered via

* Pure C++

## License

This project is licensed under the MIT License.
