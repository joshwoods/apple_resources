

- App Store Server API
-  Get Transaction Info 

Web Service Endpoint

# Get Transaction Info

Get information about a single transaction for your app.

App Store Server API 1.8+

## URL

``` source
GET https://api.storekit.itunes.apple.com/inApps/v1/transactions/{transactionId}
```

## Sandbox URL

``` source
GET https://api.storekit-sandbox.itunes.apple.com/inApps/v1/transactions/{transactionId}
```

## Path Parameters

`transactionId`

transactionId

 (Required) 

The identifier of a transaction that belongs to the customer, and which may be an original transaction identifier (originalTransactionId).

## Response Codes

` 200 ``OK`

TransactionInfoResponse

`OK`

Request succeeded.

Content-Type: application/json

` 400 ``Bad Request`

`(`InvalidTransactionIdError` | `AppTransactionIdNotSupportedError`)`

`Bad Request`

Invalid request.

Content-Type: application/json

` 401 ``Unauthorized`

`Unauthorized`

The JSON Web Token (JWT) in the authorization header is invalid. For more information, see Generating JSON Web Tokens for API requests.

` 404 ``Not Found`

TransactionIdNotFoundError

`Not Found`

The transaction identifier wasn’t found.

Content-Type: application/json

` 429 `

RateLimitExceededError

The request exceeded the rate limit.

Content-Type: application/json

` 500 ``Internal Server Error`

`(`GeneralInternalError` | `GeneralInternalRetryableError`)`

`Internal Server Error`

Server error. Try again later.

Content-Type: application/json

## Mentioned in 

App Store Server API changelog

Identifying rate limits

## Discussion

Use this endpoint to get transaction information for any transaction identifier, including original transaction identifiers. This endpoint supports all in-app purchase types, including consumable, non-consumable, non-renewing subscriptions, and auto-renewable subscriptions. It also supports transactions that your app marked as finished using finish() or finishTransaction(_:) in StoreKit.

## See Also

### Transaction information

object TransactionInfoResponse

A response that contains signed transaction information for a single transaction.

