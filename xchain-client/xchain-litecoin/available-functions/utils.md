# Utils

<!-- Generated by documentation.js. Update this documentation by updating the source code. -->

## compileMemo

Compile memo.

### Parameters

-   `memo` **[string][1]** The memo to be compiled.

Returns **[Buffer][2]** The compiled memo.

## getFee

Get the transaction fee.

### Parameters

-   `inputs` **[Array][3]&lt;UTXO>** The UTXOs.
-   `feeRate` **FeeRate** The fee rate.
-   `data` **[Buffer][2]** The compiled memo (Optional). (optional, default `null`)

Returns **[number][4]** The fee amount.

## arrayAverage

Get the average value of an array.

### Parameters

-   `array` **[Array][3]&lt;[number][4]>** 

Returns **[number][4]** The average value.

## ltcNetwork

Get Litecoin network to be used with bitcoinjs.

### Parameters

-   `network` **Network** 

Returns **Litecoin.Network** The LTC network.

## getBalance

Get the balances of an address.

### Parameters

-   `params` **AddressParams** 

Returns **[Array][3]&lt;Balance>** The balances of the given address.

## validateAddress

Validate the LTC address.

### Parameters

-   `address` **[string][1]** 
-   `network` **Network** 

Returns **[boolean][5]** `true` or `false`.

## getTxHex

Helper to get `hex` of `Tx`

It will try to get it from cache before requesting it from Sochain

### Parameters

-   `$0` **[Object][6]** 
    -   `$0.txHash`  
    -   `$0.sochainUrl`  
    -   `$0.network`  

## scanUTXOs

Scan UTXOs from sochain.

### Parameters

-   `params` **ScanUTXOParam** 
    -   `params.sochainUrl`  
    -   `params.network`  
    -   `params.address`  
    -   `params.withTxHex`   (optional, default `false`)

Returns **[Array][3]&lt;UTXO>** The UTXOs of the given address.

## buildTx

Build transcation.

### Parameters

-   `params` **BuildParams** The transaction build options.
    -   `params.amount`  
    -   `params.recipient`  
    -   `params.memo`  
    -   `params.feeRate`  
    -   `params.sender`  
    -   `params.network`  
    -   `params.sochainUrl`  
    -   `params.withTxHex`   (optional, default `false`)

Returns **Transaction** 

## broadcastTx

Broadcast the transaction.

### Parameters

-   `params` **BroadcastTxParams** The transaction broadcast options.

Returns **TxHash** The transaction hash.

## calcFee

Calculate fees based on fee rate and memo.

### Parameters

-   `feeRate` **FeeRate** 
-   `memo` **[string][1]** 

Returns **BaseAmount** The calculated fees based on fee rate and the memo.

## getDefaultFeesWithRates

Get the default fees with rates.

Returns **FeesWithRates** The default fees and rates.

## getDefaultFees

Get the default fees.

Returns **Fees** The default fees.

## getPrefix

Get address prefix based on the network.

### Parameters

-   `network` **Network** 

Returns **[string][1]** The address prefix based on the network.\*

[1]: https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String

[2]: https://nodejs.org/api/buffer.html

[3]: https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Array

[4]: https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Number

[5]: https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Boolean

[6]: https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Object