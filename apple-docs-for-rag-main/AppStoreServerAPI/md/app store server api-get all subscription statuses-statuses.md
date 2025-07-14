

- App Store Server API
-  Get All Subscription Statuses 

Web Service Endpoint

# Get All Subscription Statuses

Get the statuses for all of a customer’s auto-renewable subscriptions in your app.

App Store Server API 1.0+

## URL

``` source
GET https://api.storekit.itunes.apple.com/inApps/v1/subscriptions/{transactionId}
```

## Sandbox URL

``` source
GET https://api.storekit-sandbox.itunes.apple.com/inApps/v1/subscriptions/{transactionId}
```

## Path Parameters

`transactionId`

transactionId

 (Required) 

The identifier of a transaction that belongs to the customer, and which may be an original transaction identifier (originalTransactionId).

## Query Parameters

`status`

`[`status`]`

An optional filter that indicates the status of subscriptions to include in the response. Your query may specify more than one `status` query parameter.

## Response Codes

` 200 ``OK`

StatusResponse

`OK`

Request succeeded.

Content-Type: application/json

` 400 ``Bad Request`

`(`InvalidAppIdentifierError` | `InvalidTransactionIdError` | `InvalidStatusError`)`

`Bad Request`

Content-Type: application/json

` 401 ``Unauthorized`

`Unauthorized`

The JSON Web Token (JWT) in the authorization header is invalid. For more information, see Generating JSON Web Tokens for API requests.

` 404 ``Not Found`

`(`AccountNotFoundError` | `AccountNotFoundRetryableError` | `AppNotFoundError` | `AppNotFoundRetryableError` | `TransactionIdNotFoundError`)`

`Not Found`

Content-Type: application/json

` 429 `

RateLimitExceededError

The request exceeded the rate limit.

Content-Type: application/json

` 500 ``Internal Server Error`

`(`GeneralInternalError` | `GeneralInternalRetryableError`)`

`Internal Server Error`

Content-Type: application/json

## Mentioned in 

App Store Server API changelog

Identifying rate limits

## Discussion

This API returns the status for all of the customer’s subscriptions, organized by their subscription group identifier.

Specify multiple values for the `status` query parameter to get a response that contains subscriptions with statuses that match any of the values. For example, the following request returns subscriptions that are active (status value of `1`) and subscriptions that are in the Billing Grace Period (status value of `4`):

```
GET https://api.storekit.itunes.apple.com/inApps/v1/subscriptions/{transactionId}?status=1&status=4
```

## See Also

### Subscription status

object StatusResponse

A response that contains status information for all of a customer’s auto-renewable subscriptions in your app.

