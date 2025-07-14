

- App Store Server API
-  Get Refund History V1 Deprecated

Web Service Endpoint

# Get Refund History V1

Get a list of up to 50 of a customer’s refunded in-app purchases for your app.

App Store Server API 1.1–1.6Deprecated

Deprecated

Use Get Refund History instead.

## URL

``` source
GET https://api.storekit.itunes.apple.com/inApps/v1/refund/lookup/{originalTransactionId}
```

## Sandbox URL

``` source
GET https://api.storekit-sandbox.itunes.apple.com/inApps/v1/refund/lookup/{originalTransactionId}
```

## Path Parameters

`originalTransactionId`

originalTransactionId

 (Required) 

The original transaction identifier for a transaction that belongs to the customer.

## Response Codes

` 200 ``OK`

RefundLookupResponse

`OK`

Request succeeded.

Content-Type: application/json

` 400 ``Bad Request`

InvalidOriginalTransactionIdError

`Bad Request`

The request is invalid. Check the specific error message for further information.

Content-Type: application/json

` 401 ``Unauthorized`

`Unauthorized`

The JSON Web Token (JWT) in the authorization header is invalid. For more information, see Generating JSON Web Tokens for API requests.

` 404 ``Not Found`

OriginalTransactionIdNotFoundError

`Not Found`

The request is invalid. Check the specific error message for further information.

Content-Type: application/json

` 429 `

RateLimitExceededError

Content-Type: application/json

` 500 ``Internal Server Error`

`(`GeneralInternalError` | `GeneralInternalRetryableError`)`

`Internal Server Error`

The request failed. This may be due to a temporary outage. Check the specific error message for further information.

Content-Type: application/json

## Mentioned in 

App Store Server API changelog

Identifying rate limits

## Discussion

Call this endpoint to get a customer’s refund history for your app. The response (RefundLookupResponse) includes up to 50 of the customer’s most-recently refunded transactions, based on the revocationDate.

Note

To get the complete refund history, use Get Refund History.

To call this endpoint, provide any original transaction identifier (originalID) for any of the customer’s in-app purchases. The response only includes App Store-approved refunds for any product type: consumable, non-consumable, auto-renewable subscriptions, and non-renewing subscriptions. For more information about product types, see In-app purchase.

The information in the response is the same as the information in one or more `REFUND` notifications (notificationType) from App Store Server Notifications. Use this API to retrieve any refund notifications you may have missed, such as during a server outage.

A successful response may have an empty `signedTransactions` array if the customer hasn’t received any App Store-approved refunds. To identify the date and reason code for a refund, see `revocationDate` and `revocationReason` in the JWSTransactionDecodedPayload.

The App Store Server API returns information based on the customer’s in-app purchase history regardless of whether the customer installs, removes, or reinstalls the app on their devices.

## See Also

### Refund lookup

Get Refund History

Get a paginated list of all of a customer’s refunded in-app purchases for your app.

object RefundHistoryResponse

A response that contains an array of signed JSON Web Signature (JWS) refunded transactions, and paging information.

object RefundLookupResponse

A response that contains an array of signed JSON Web Signature (JWS) transactions.

Deprecated

