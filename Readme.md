## Query the tokens

### description

> Query the tokens that users are interested in

Method: GET

Path:  https://apis.tomo.inc/sky/api/socialLogin/teleGram/wallet/favouriteTokens

> example

> 200 Response

```json
{
  "result": [
    {
      "createdTime": "2019-08-24T14:15:22Z",
      "updatedTime": "2019-08-24T14:15:22Z",
      "id": 0,
      "name": "string",
      "displayName": "string",
      "symbol": "string",
      "imageUrl": "string",
      "decimals": 0,
      "chain": "string",
      "isNative": true,
      "isTomoji": true,
      "tomojiId": 0,
      "address": "string",
      "priceUsd": "string",
      "priceChangeH24": 0.1,
      "volumeH24": "string",
      "marketCapUsd": "string",
      "poolAddress": "string",
      "supportRango": true,
      "groupId": "string"
    }
  ],
  "code": 0,
  "message": "string"
}
```

### 

## Title:  Update the tokens that users follow

 Method: POST

 Path:  /api/socialLogin/teleGram/wallet/favouriteTokens

 Body Request parameters

```json
{
  "userId": 0,
  "tokens": [
    "string"
  ]
}
```

### Request parameters

| name | position | type                                                                | required | description |
| ---- | -------- | ------------------------------------------------------------------- | -------- | ----------- |
| body | body     | [UpdateUserFavouriteTokensDTO](#schemaupdateuserfavouritetokensdto) | false    | none        |

> example

> 200 Response

```json
{
  "result": true,
  "code": 0,
  "message": "string"
}
```

### 

## Title:  K-line chart data

Method: GET

Path:  /api/socialLogin/teleGram/{tokenName}/OHLCV

### Request parameters

| name      | position | type   | required | description |
| --------- | -------- | ------ | -------- | ----------- |
| tokenName | path     | string | true     | none        |
| interval  | query    | string | true     | none        |

#### menu value

| property | value          |
| -------- | -------------- |
| interval | hour           |
| interval | four_hour      |
| interval | day            |
| interval | week           |
| interval | month          |
| interval | minute         |
| interval | five_minute    |
| interval | fifteen_minute |

> example

> 200 Response

```json
{
  "result": [
    {
      "timestamp": 0,
      "open": 0.1,
      "high": 0.1,
      "low": 0.1,
      "close": 0.1,
      "volume": 0.1
    }
  ],
  "code": 0,
  "message": "string"
}
```

## Title:  Chain maintained based on chains.json, check tokens

Method: GET

Path:  /api/socialLogin/teleGram/wallet/trendingTokens

> example

> 200 Response

```json
{
  "result": [
    {
      "createdTime": "2019-08-24T14:15:22Z",
      "updatedTime": "2019-08-24T14:15:22Z",
      "id": 0,
      "name": "string",
      "displayName": "string",
      "symbol": "string",
      "imageUrl": "string",
      "decimals": 0,
      "chain": "string",
      "isNative": true,
      "isTomoji": true,
      "tomojiId": 0,
      "address": "string",
      "priceUsd": "string",
      "priceChangeH24": 0.1,
      "volumeH24": "string",
      "marketCapUsd": "string",
      "poolAddress": "string",
      "supportRango": true,
      "groupId": "string"
    }
  ],
  "code": 0,
  "message": "string"
}
```

## Title: Search for all tokens

Method: GET

Path: /api/socialLogin/teleGram/wallet/tokens

> example

> 200 Response

```json
{
  "result": [
    {
      "createdTime": "2019-08-24T14:15:22Z",
      "updatedTime": "2019-08-24T14:15:22Z",
      "id": 0,
      "name": "string",
      "displayName": "string",
      "symbol": "string",
      "imageUrl": "string",
      "decimals": 0,
      "chain": "string",
      "isNative": true,
      "isTomoji": true,
      "tomojiId": 0,
      "address": "string",
      "priceUsd": "string",
      "priceChangeH24": 0.1,
      "volumeH24": "string",
      "marketCapUsd": "string",
      "poolAddress": "string",
      "supportRango": true,
      "groupId": "string"
    }
  ],
  "code": 0,
  "message": "string"
}
```

## Title: Query tokens based on address and chain

Method: GET

Path:  /api/socialLogin/teleGram/wallet/tokens/search

### Request parameters

| name    | position | type   | required | description |
| ------- | -------- | ------ | -------- | ----------- |
| content | query    | string | true     | none        |
| chain   | query    | string | false    | none        |

> example

> 200 Response

```json
{
  "result": [
    {
      "createdTime": "2019-08-24T14:15:22Z",
      "updatedTime": "2019-08-24T14:15:22Z",
      "id": 0,
      "name": "string",
      "displayName": "string",
      "symbol": "string",
      "imageUrl": "string",
      "decimals": 0,
      "chain": "string",
      "isNative": true,
      "isTomoji": true,
      "tomojiId": 0,
      "address": "string",
      "priceUsd": "string",
      "priceChangeH24": 0.1,
      "volumeH24": "string",
      "marketCapUsd": "string",
      "poolAddress": "string",
      "supportRango": true,
      "groupId": "string"
    }
  ],
  "code": 0,
  "message": "string"
}
```

### 

## Title: tg market > all assets  (tg market. all assets)

Method: GET

Path: /api/socialLogin/teleGram/wallet/selectedTokens

> example

> 200 Response

```json
{
  "result": [
    {
      "createdTime": "2019-08-24T14:15:22Z",
      "updatedTime": "2019-08-24T14:15:22Z",
      "id": 0,
      "name": "string",
      "displayName": "string",
      "symbol": "string",
      "imageUrl": "string",
      "decimals": 0,
      "chain": "string",
      "isNative": true,
      "isTomoji": true,
      "tomojiId": 0,
      "address": "string",
      "priceUsd": "string",
      "priceChangeH24": 0.1,
      "volumeH24": "string",
      "marketCapUsd": "string",
      "poolAddress": "string",
      "supportRango": true,
      "groupId": "string"
    }
  ],
  "code": 0,
  "message": "string"
}
```

### 

## Title: Retrieve only one token based on its name

Method: GET

Path:  /api/socialLogin/teleGram/getByName

### Request parameters

| name      | position | type   | required | description |
| --------- | -------- | ------ | -------- | ----------- |
| tokenName | query    | string | true     | none        |

> example

> 200 Response

```json
{
  "result": {
    "createdTime": "2019-08-24T14:15:22Z",
    "updatedTime": "2019-08-24T14:15:22Z",
    "id": 0,
    "name": "string",
    "displayName": "string",
    "symbol": "string",
    "imageUrl": "string",
    "decimals": 0,
    "chain": "string",
    "isNative": true,
    "isTomoji": true,
    "tomojiId": 0,
    "address": "string",
    "priceUsd": "string",
    "priceChangeH24": 0.1,
    "volumeH24": "string",
    "marketCapUsd": "string",
    "poolAddress": "string",
    "supportRango": true,
    "groupId": "string"
  },
  "code": 0,
  "message": "string"
}
```

### 

## 

## Title: Signature source data (raw transaction)

Method: POST

Path:  /api/socialLogin/projectWallet/solana/signRawTransaction   

Body Request parameters

```json
{
  "rawTransaction": "string"
}
```

### Request parameters

| name | position | type                                                                      | required | description |
| ---- | -------- | ------------------------------------------------------------------------- | -------- | ----------- |
| body | body     | [SolanaSignRawTransactionRequest](#schemasolanasignrawtransactionrequest) | false    | none        |

> example

> 200 Response

```json
{
  "result": "string",
  "code": 0,
  "message": "string"
}
```

### 

## Title: Send raw transaction source data for TY transactions

Method: POST

Path:  /api/socialLogin/projectWallet/ethereum/sendRawTransaction   

Body Request parameters

```json
{
  "rawTransaction": "string",
  "chainId": 0,
  "rpc": "string"
}
```

### Request parameters

| name | position | type                                                                          | required | description |
| ---- | -------- | ----------------------------------------------------------------------------- | -------- | ----------- |
| body | body     | [EthereumSendRawTransactionRequest](#schemaethereumsendrawtransactionrequest) | false    | none        |

> example

> 200 Response

```json
{
  "result": "string",
  "code": 0,
  "message": "string"
}
```

### 

## Title: Sign the transaction and send the transaction

Method: POST

Path: /socialLogin/projectWallet/bitcoin/signPsbtAndPush   

Body Request parameters

```json
{
  "networkType": "MAINNET | TESTNET | SIGNET",
  "addressType": "P2PKH | P2WPKH | P2TR |P2SH",
  "psbtHex": "string",
  "autoFinalized": true
}
```

### Request parameters

| name | position | type                                                    | required | description |
| ---- | -------- | ------------------------------------------------------- | -------- | ----------- |
| body | body     | [BitcoinSignPsbtRequest](#schemabitcoinsignpsbtrequest) | false    | none        |

> example

> 200 Response

```json
{
  "result": "string",
  "code": 0,
  "message": "string"
}
```

### 

## Title: Send BTC transaction

Method: POST

Path:  /api/socialLogin/projectWallet/bitcoin/pushTransaction

Body Request parameters

```json
{
  "networkType": "MAINNET | TESTNET | SIGNET",
  "rawTransaction": "string"
}
```

### Request parameters

| name | position | type                                                                  | required | description |
| ---- | -------- | --------------------------------------------------------------------- | -------- | ----------- |
| body | body     | [BitcoinPushTransactionRequest](#schemabitcoinpushtransactionrequest) | false    | none        |

> example

> 200 Response

```json
{
  "result": "string",
  "code": 0,
  "message": "string"
}
```

### 

## Title: Create a transaction to send BTC

Method:  POST

Path: /api/socialLogin/projectWallet/bitcoin/createSendBitcoinPsbt 

Body Request parameters

```json
{
  "networkType": "MAINNET | TESTNET | SIGNET",
  "addressType": "P2PKH | P2WPKH | P2TR |P2SH",
  "toAddress": "string",
  "amount": 0,
  "feeRate": 0.1
}
```

### Request parameters

| name | position | type                                                                              | required | description |
| ---- | -------- | --------------------------------------------------------------------------------- | -------- | ----------- |
| body | body     | [BitcoinCreateSendBitcoinPsbtRequest](#schemabitcoincreatesendbitcoinpsbtrequest) | false    | none        |

> example

> 200 Response

```json
{
  "result": {
    "property1": {},
    "property2": {}
  },
  "code": 0,
  "message": "string"
}
```

### 

# 

## Title: Send a code to the email address to bind it

Method: POST

Path:  /api/socialLogin/projectUser/bindEmailCodeVerify

Body Request parameters

```json
{
  "email": "string",
  "code": "string"
}
```

### Request parameters

| name | position | type                                                | required | description |
| ---- | -------- | --------------------------------------------------- | -------- | ----------- |
| body | body     | [UserEmailBindCodeDTO](#schemauseremailbindcodedto) | false    | none        |

> example

> 200 Response

```json
{
  "result": true,
  "code": 0,
  "message": "string"
}
```

### 

## Title: Verify and bind email address

Method : GET

Path:  /api/socialLogin/projectUser/bindEmailCode

### Request parameters

| name  | position | type   | required | description |
| ----- | -------- | ------ | -------- | ----------- |
| email | query    | string | true     | none        |

> example

> 200 Response

```json
{
  "result": true,
  "code": 0,
  "message": "string"
}
```

### 

## Title: Etheuem transaction signature

Method: POST

Path:  /api/socialLogin/projectWallet/ethereum/signTransaction

Body Request parameters

```json
{
  "transaction": {
    "to": "string",
    "value": "string",
    "data": "string",
    "nonce": 0,
    "gas": "string",
    "gasPrice": "string",
    "maxFeePerGas": "string",
    "maxPriorityFeePerGas": "string"
  }
}
```

### Request parameters

| name | position | type                                                                    | required | description |
| ---- | -------- | ----------------------------------------------------------------------- | -------- | ----------- |
| body | body     | [EthereumSignTransactionRequest](#schemaethereumsigntransactionrequest) | false    | none        |

> example

> 200 Response

```json
{
  "result": "string",
  "code": 0,
  "message": "string"
}
```

### 

## Title: Send raw transaction source data for TY transactions

Method: Post
Path:  /api/socialLogin/projectWallet/ethereum/sendRawTransaction

Body Request parameters

```json
{
  "rawTransaction": "string",
  "chainId": 0,
  "rpc": "string"
}
```

### Request parameters

| name | position | type                                                                          | required | description |
| ---- | -------- | ----------------------------------------------------------------------------- | -------- | ----------- |
| body | body     | [EthereumSendRawTransactionRequest](#schemaethereumsendrawtransactionrequest) | false    | none        |

> example

> 200 Response

```json
{
  "result": "string",
  "code": 0,
  "message": "string"
}
```

### 

## Title: Customize assets, add new assets

Method: POST

Path:  /v1/asset/add

Description: Add token asset for user

> Body Request parameters

```json
{
  "chain_id": 0,
  "decimals": 30,
  "image": "string",
  "name": "string",
  "symbol": "string",
  "token": "string"
}
```

### Request parameters

| name          | position | type                                      | required | description   |
| ------------- | -------- | ----------------------------------------- | -------- | ------------- |
| Authorization | header   | string                                    | false    | Authorization |
| body          | body     | [AddTokenRequest](#schemaaddtokenrequest) | false    | none          |

> example

> 200 Response

```json
{
  "code": 0,
  "message": "string"
}
```

## Title: Get token asset for user

Methd: GET

Path:  /v1/asset/all

Description: Get token asset for user

### Request parameters

| name          | position | type           | required | description   |
| ------------- | -------- | -------------- | -------- | ------------- |
| chain_ids     | query    | array[integer] | false    | chain ids     |
| page          | query    | integer        | false    | page          |
| pagesize      | query    | integer        | false    | pagesize      |
| Authorization | header   | string         | false    | Authorization |

> example

> 200 Response

```json
{
  "code": 0,
  "data": [
    {
      "chain_id": 0,
      "created_at": 0,
      "decimals": 0,
      "id": 0,
      "image": "string",
      "name": "string",
      "symbol": "string",
      "token": "string",
      "uid": 0
    }
  ],
  "message": "string"
}
```

## Title: Del token asset

Method: DELETE

Path:  /v1/asset/del/{chain_id}/{token}

Description: Del token asset for user

### Request parameters

| name          | position | type    | required | description   |
| ------------- | -------- | ------- | -------- | ------------- |
| chain_id      | path     | integer | true     | chain id      |
| token         | path     | string  | true     | token address |
| Authorization | header   | string  | false    | Authorization |

> example

> 200 Response

```json
{
  "code": 0,
  "message": "string"
}
```

## Title: Check if the device has a passkey

Method: GET

Path:  /v2/passkey/check/{device_no}

Description: check passkey v2

### Request parameters

| name          | position | type   | required | description   |
| ------------- | -------- | ------ | -------- | ------------- |
| device_no     | path     | string | true     | device no     |
| Authorization | header   | string | false    | Authorization |

> example

> 200 Response

```json
{
  "code": 0,
  "data": {
    "is_exists": true
  },
  "message": "string"
}
```

## Title: create passkey v2

Method: POST

Path: /v2/passkey/create

Description:  Submit Pubkey to table

> Body Request parameters

```json
{
  "device_no": "string",
  "pubkey": "string"
}
```

### Request parameters

| name          | position | type                                                    | required | description   |
| ------------- | -------- | ------------------------------------------------------- | -------- | ------------- |
| Authorization | header   | string                                                  | false    | Authorization |
| body          | body     | [PasskeyV2CreateRequest](#schemapasskeyv2createrequest) | false    | none          |

> example

> 200 Response

```json
{
  "code": 0,
  "message": "string"
}
```

## Title: validate passkey v2

Method: POST

Path: /v2/passkey/validate

Description: Submit message & sign to validate

> Body Request parameters

```json
{
  "device_no": "string",
  "message": "string",
  "sig": "string"
}
```

### Request parameters

| name          | position | type                                                        | required | description   |
| ------------- | -------- | ----------------------------------------------------------- | -------- | ------------- |
| Authorization | header   | string                                                      | false    | Authorization |
| body          | body     | [PasskeyV2ValidateRequest](#schemapasskeyv2validaterequest) | false    | none          |

> example

> 200 Response

```json
{
  "code": 0,
  "data": {
    "key": "string"
  },
  "message": "string"
}
```

## Title: change passwd

Method: POST

Path: /v1/payment/passwd/change

Description: change passwd is exist

> Body Request parameters

```json
{
  "new_passwd": "string",
  "old_passwd": "string"
}
```

### Request parameters

| name          | position | type                                                            | required | description   |
| ------------- | -------- | --------------------------------------------------------------- | -------- | ------------- |
| Authorization | header   | string                                                          | false    | Authorization |
| body          | body     | [PaymentPasswdChangeRequest](#schemapaymentpasswdchangerequest) | false    | none          |

> example

> 200 Response

```json
{
  "code": 0,
  "message": "string"
}
```

## Title: check passwd

Method: GET

Path: /v1/payment/passwd/check

Description:  check passwd is exist

### Request parameters

| name          | position | type   | required | description   |
| ------------- | -------- | ------ | -------- | ------------- |
| Authorization | header   | string | false    | Authorization |

> example

> 200 Response

```json
{
  "code": 0,
  "data": {
    "is_exists": true
  },
  "message": "string"
}
```

## Title: set passwd

Method: POST

Path: /v1/payment/passwd/set

Description: set passwd is exist

> Body Request parameters

```json
{
  "passwd": "string"
}
```

### Request parameters

| name          | position | type                                                | required | description   |
| ------------- | -------- | --------------------------------------------------- | -------- | ------------- |
| Authorization | header   | string                                              | false    | Authorization |
| body          | body     | [PaymentPasswdRequest](#schemapaymentpasswdrequest) | false    | none          |

> example

> 200 Response

```json
{
  "code": 0,
  "message": "string"
}
```

## Title:  validate passwd

Method: POST

Path: /v1/payment/passwd/validate

Description: validate passwd is exist

> Body Request parameters

```json
{
  "passwd": "string"
}
```

### Request parameters

| name          | position | type                                                | required | description   |
| ------------- | -------- | --------------------------------------------------- | -------- | ------------- |
| Authorization | header   | string                                              | false    | Authorization |
| body          | body     | [PaymentPasswdRequest](#schemapaymentpasswdrequest) | false    | none          |

> example

> 200 Response

```json
{
  "code": 0,
  "message": "string"
}
```

## Title: get all token

Method: GET

Path: /v1/token/balance

Description: get all token(contain native token & contract token)

### Request parameters

| name           | position | type   | required | description         |
| -------------- | -------- | ------ | -------- | ------------------- |
| evm_address    | query    | string | true     | user evm address    |
| solana_address | query    | string | true     | user solana address |
| Authorization  | header   | string | false    | Authorization       |

> example

> 200 Response

```json
{
  "code": 0,
  "data": [
    {
      "balance": "string",
      "chain_id": 0,
      "contract": "string",
      "decimals": 0,
      "image": "string",
      "is_native": true,
      "mercuryo_support": "string",
      "name": "string",
      "price": 0,
      "ramp_support": "string",
      "symbol": "string"
    }
  ],
  "message": "string"
}
```

# 

## Title: generate public key

Method: Post

Path:  /v2/reg/{device_no}

Description: generate public key

### Request parameters

| name          | position | type   | required | description   |
| ------------- | -------- | ------ | -------- | ------------- |
| device_no     | path     | string | true     | device no     |
| Authorization | header   | string | false    | Authorization |

> example

> 200 Response

```json
{
  "code": 0,
  "data": {
    "pubkey": "string"
  },
  "message": "string"
}
```

## Title: sign message

Method: Post

Path:  /v2/sign

Description: sign message

> Body Request parameters

```json
{
  "device_no": "string",
  "message": "string"
}
```

### Request parameters

| name          | position | type                                | required | description   |
| ------------- | -------- | ----------------------------------- | -------- | ------------- |
| Authorization | header   | string                              | false    | Authorization |
| body          | body     | [DeviceSigReq](#schemadevicesigreq) | false    | none          |

> example

> 200 Response

```json
{
  "code": 0,
  "data": {
    "signature": "string"
  },
  "message": "string"
}
```

## Title: query token details

Method: GET

Path: /prod/avp_tomoji/v4/memes-overview

Description: query token details

### Request parameters

| name    | position | type   | required | description |
| ------- | -------- | ------ | -------- | ----------- |
| address | query    | string | true     | none        |
| chain   | query    | string | true     | none        |

> example

> 10000 Response

```json
{
  "code": 10000,
  "message": "Success",
  "result": {
    "address": "0x8290333cef9e6d528dd5618fb97a76f268f3edd4",
    "decimals": 18,
    "symbol": "ANKR",
    "name": "Ankr Network",
    "extensions": {
      "twitter": "https://twitter.com/ankr",
      "website": "https://stakefi.ankr.com",
      "telegram": "https://t.me/ankrnetwork"
    },
    "logoURI": "https://coin-images.coingecko.com/coins/images/4324/small/U85xTl2.png?1696504928",
    "liquidity": 154202.88165825416,
    "price": 0.02630104,
    "supply": 10000000000,
    "mc": 256711503,
    "history24hPrice": 0,
    "priceChange24hPercent": 5.753056067701485,
    "fdvUsd": 263147232.108125,
    "high24h": 0.02657743,
    "low24h": 0.02488059
  }
}
```
