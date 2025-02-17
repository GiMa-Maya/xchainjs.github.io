# Wallet

<!-- Generated by documentation.js. Update this documentation by updating the source code. -->

## Wallet

Wallet Class for managing all xchain-\* wallets with a mnemonic seed.

### Parameters

-   `phrase`  mnemonic phrase
-   `thorchainQuery`  
-   `thorchainCache`  an instance of the ThorchainCache (could be pointing to stagenet,testnet,mainnet)

### getAllBalances

Fetch balances for all wallets

Returns **any** AllBalances\[]

### executeSwap

-   **See: ThorchainAMM.doSwap()
    **

Executes a Swap from THORChainAMM.doSwap()

#### Parameters

-   `swap`  object with all the required details for a swap.

Returns **any** transaction details and explorer url

### validateSwap

Validate swap object

#### Parameters

-   `swap`  swap parameters

### swapRuneTo

Function handles all swaps from Rune to asset

#### Parameters

-   `swap`  swap parameters

Returns **any** tx submitted object

### swapNonRune

Function handles all swaps from Non Rune

#### Parameters

-   `swap`  swap object

Returns **any** TxSubmitted object

### addLiquidity

Function handles liquidity Add
BASED OFF [https://dev.thorchain.or›g/thorchain-dev/network/memos][1]

#### Parameters

-   `params`  input parameters needed to add liquidity

Returns **any** transaction details submitted

### withdrawLiquidity

Function handles liquidity Withdraw

#### Parameters

-   `params`  parameters required for liquidity position

Returns **any** object with tx response, url and wait time in seconds

### addSavers

#### Parameters

-   `assetAmount`  amount to add
-   `memo`  memo required
-   `toAddress`  
-   `waitTimeSeconds`  expected wait for the transaction to be processed

### withdrawSavers

#### Parameters

-   `dustAssetAmount`  
-   `memo`  memo required
-   `toAddress`  
-   `waitTimeSeconds`  expected wait for the transaction to be processed
-   `assetAmount`  amount to withdraw

### addAssetLP

Function handles liquidity add for all non rune assets

#### Parameters

-   `params`  parameters for add liquidity
-   `constructedMemo`  memo needed for thorchain
-   `assetClient`  passing XchainClient
-   `waitTimeSeconds`  wait time for the tx to be confirmed
-   `inboundAsgard`  inbound Asgard address for the LP

Returns **any** tx object

### withdrawAssetLP

Function handles liquidity Withdraw for Non rune assets

#### Parameters

-   `params`  parameters for withdraw liquidity
-   `constructedMemo`  memo needed for thorchain execution
-   `assetClient`  asset client to call transfer
-   `waitTimeSeconds`  return back estimated wait
-   `inboundAsgard`  destination address

Returns **any** tx object

### addRuneLP

Function handles liquidity Add for Rune only

#### Parameters

-   `params`  deposit parameters
-   `memo`  memo needed to withdraw lp
-   `thorchainClient`  
-   `waitTimeSeconds`  

Returns **any** tx object

### withdrawRuneLP

Function handles liquidity Withdraw for Rune only

#### Parameters

-   `params`  withdraw parameters
-   `memo`  memo needed to withdraw lp
-   `thorchainClient`  
-   `waitTimeSeconds`  

Returns **any** tx object

[1]: https://dev.thorchain.or›g/thorchain-dev/network/memos
