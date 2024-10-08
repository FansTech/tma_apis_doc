## Title: Query the tokens that users are interested in

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

 Path:  https://apis.tomo.inc/sky/api/socialLogin/teleGram/wallet/favouriteTokens

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

Path:  https://apis.tomo.inc/sky/api/socialLogin/teleGram/{tokenName}/OHLCV

Description: Query chart data by time period; interval: The following values need to be passed in

like： 
DAY 
WEEK 
MONTH 
HOUR 
FOUR_HOUR
MINUTE
FIVE_MINUTE
FIFTEEN_MINUTE

### Request parameters

| name      | position | type   | required | description |
| --------- | -------- | ------ | -------- | ----------- |
| tokenName | path     | string | true     | none        |
| interval  | query    | string | true     | none        |

#### menu value

| property | value          |
| -------- | -------------- |
| interval | HOUR           |
| interval | FOUR_HOUR      |
| interval | DAY            |
| interval | WEEK           |
| interval | MONTH          |
| interval | MINUTE         |
| interval | FIVE_MINUTE    |
| interval | FIFTEEN_MINUTE |

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

## Title:  Chain maintained based on chains.json,query tokens（trending）

Method: GET

Path:  https://apis.tomo.inc/sky/api/socialLogin/teleGram/wallet/trendingTokens

Description: Query trending data 

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

Path: https://apis.tomo.inc/sky/api/socialLogin/teleGram/wallet/tokens

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

Path:  https://apis.tomo.inc/sky/api/socialLogin/teleGram/wallet/tokens/search

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

Path: https://apis.tomo.inc/sky/api/socialLogin/teleGram/wallet/selectedTokens

Description: Query tg market data

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

Path:  https://apis.tomo.inc/sky/api/socialLogin/teleGram/getByName

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

# 

## Title: Send a code to the email address to bind it

Method: POST

Path:  https://apis.tomo.inc/sky/api/socialLogin/projectUser/bindEmailCodeVerify

Body Request parameters

```json
{
  "email": "string",
  "code": "string",
  "tradePassword": "string"
}
```

### Request parameters

| name | position | type                                                | required | description |
| ---- | -------- | --------------------------------------------------- | -------- | ----------- |
| body | body     | [TgEmailCodeBindDTO](#schematgemailcodebinddto) | false    | none        |

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

Path:  https://apis.tomo.inc/sky/api/socialLogin/projectUser/bindEmailCode


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




## Title: Customize assets, add new assets

Method: POST

Path:  https://apis.tomo.inc/wind/v1/asset/add

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

Path:  https://apis.tomo.inc/wind/v1/asset/all

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

Path:  https://apis.tomo.inc/wind/v1/asset/del/{chain_id}/{token}

Description: Del token asset for user by chain_id and token

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

Path:  https://apis.tomo.inc/wind/v2/passkey/check/{device_no}

Description: check passkey v2 by device_no

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

Path: https://apis.tomo.inc/wind/v2/passkey/create

Description:  create passkey v2 by device_no and pubkey

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

Path: https://apis.tomo.inc/wind/v2/passkey/validate

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

Path: https://apis.tomo.inc/wind/v1/payment/passwd/change

Description: change passwd 

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

Path: https://apis.tomo.inc/wind/v1/payment/passwd/check

Description:  Verify the password

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

Path: https://apis.tomo.inc/wind/v1/payment/passwd/set

Description: set passwd 

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

Path: https://apis.tomo.inc/wind/v1/payment/passwd/validate

Description: Verify the password if it exists

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

Path: https://apis.tomo.inc/wind/v1/token/balance

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

Path:  https://apis.tomo.inc/rain/v2/reg/{device_no}

Description: generate public key through device_no

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

Path:  https://apis.tomo.inc/rain/v2/sign

Description: Signature through the device_no

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

Path: https://apis.tomo.inc/cloud/v4/memes-overview


Description: Query the token through the address and chain

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
## Verify token and return tonaddress

Path: https://apis.tomo.inc/wind/v1/ton/address

Method:GET

Description: Verify token and return tonaddress

> Body Request parameters

### Request parameters

| name          | position | type   | required | description |
| ------------- | -------- | ------ | -------- | ----------- |
| Authorization | header   | string | true     | none        |

> example

> success

```json
{
  "code": 8000,
  "message": "OK",
  "data": {
    "ton_address": "UQDsuld919O2n6mxq-HtIv7Xug7szHELCOfe70DtEigdisJ1"
  }
}
```

## Swap token

Path: https://apis.tomo.inc/sun/v1/buildTx

Method:GET

Description: Query Swap Token

> Body Request parameters

### Request parameters

| name          | position | type   | required | description |
| ------------- | -------- | ------ | -------- | ----------- |
| fromChainid | query   | uint64 | true     | none        |
| toChainid | query   | uint64 | true     | none        |
| fromAddress | query   | string | false     | none        |
| toAddress | query   | string | false     | none        |
| amount | query   | string | true     | none        |
| slippage | query   | uint64 | true     | 1 ~ 1000     |
| fromWalletAddress | query   | string | true     | from wallet address    |
| toWalletAddress | query   | string | true     | to wallet address     |


> example

> 200 Response

```json
{
  "code": 0,
  "data": {
    "dex_name": "string",
    "receive_amount": "string",
    "min_receive_amount": "string",
    "origin_data": "string",
    "source": "rango",
    "transaction": {
      "approve_data": "string",
      "approve_to": "string",
      "data": "string",
      "from": "string",
      "gas": "string",
      "gasPrice": "string",
      "maxFeePerGas": "string",
      "maxGasPrice": "string",
      "maxPriorityFeePerGas": "string",
      "priorityGasPrice": "string",
      "to": "string",
      "value": "string"
    }
  },
  "message": "string"
}
```

> other Response

```
{
  "code": 0,
  "message": "string"
}
```
## Special instructions:
All interfaces need to add a token to the header

> example


Authorization: Bearer eyJraWQiOiIyBzMxMjA2MTcySiIsInR5cC26IkpXVCIsImFsZyI6IlJTMjU2In0.eyJhcHAiOiJ0b21vIiwidXNlcl9pZCI6Nzg2NzExLCJleHAiOjE3MjY5NjU3MjAsImlhdCI6MTcyNDM3MzcyMCwiY2xpZW50X2lkIjoiSVV2d0VQZXVtV0d3MFRPT1cxWDlvOGhIaDRETmVNNWpvY1BPNkJVQTdJVU1FVWhkekozUG9MYVBwbFJ0WE92MVl5cEVLa2FIWWZxT3IzRHlxcWhkaVRPZSIsInVzZXJuYW1lIjoidGVsZWdyYW1Ab2xpdmVyb28wbyJ9.PHb9U86KS79_-bVjHVZqx6xY80Fg9MmnQ33Tl5H_A5yN7JVMTyyLD5SsoMSnx4ykJH1an5zKKztsk_nmJg_np-D4h761SS0MAzerzhOnl6Qdvq2FKfxioU4U2Ky4JhzdeksFsnamXALg7Vc-EUJ0B4sUJK7SjmzMdPGT7Yr8lL2
