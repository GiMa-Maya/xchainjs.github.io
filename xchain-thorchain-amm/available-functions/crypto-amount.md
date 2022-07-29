# Crypto Amount

<!-- Generated by documentation.js. Update this documentation by updating the source code. -->

## CryptoAmount

Utility Class to combine an amount (asset/base) with the Asset

### Parameters

-   `amount`  
-   `asset`  

### check

This guard protects against trying to perform math with different assets

Example.
const x = new CryptoAmount(baseAmount(1),AssetBTC)
const y = new CryptoAmount(baseAmount(1),AssetETH)

x.plus(y) &lt;- will throw error "cannot perform math on 2 diff assets BTC.BTC ETH.ETH

#### Parameters

-   `v`  CryptoNumeric