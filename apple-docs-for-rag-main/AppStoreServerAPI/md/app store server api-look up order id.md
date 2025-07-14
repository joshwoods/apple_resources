

- App Store Server API
-  Look Up Order ID 

Web Service Endpoint

# Look Up Order ID

Get a customer’s in-app purchases from a receipt using the order ID.

App Store Server API 1.1+

## URL

``` source
GET https://api.storekit.itunes.apple.com/inApps/v1/lookup/{orderId}
```

## Path Parameters

`orderId`

orderId

 (Required) 

The order ID for in-app purchases that belong to the customer.

## Response Codes

` 200 ``OK`

OrderLookupResponse

`OK`

Request succeeded.

Content-Type: application/json

` 400 ``Bad Request`

GeneralBadRequestError

`Bad Request`

The request is invalid and can’t be accepted.

Content-Type: application/json

` 401 ``Unauthorized`

`Unauthorized`

The JSON Web Token (JWT) in the authorization header is invalid. For more information, see Generating JSON Web Tokens for API requests.

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

Important

This endpoint isn’t available in the sandbox environment.

Call this endpoint to identify and validate a customer’s in-app purchases, based on their order ID.

When a customer contacts you for support, ask for their order ID and use that value to call this endpoint. Customers can retrieve their order IDs from their purchase history on the App Store; for more information, see See your purchase history for the App Store, iTunes store, and more. The App Store also sends customers an email receipt with an order ID each time they make in-app purchases.

A successful response with an OrderLookupStatus value of `0` contains an array of one or more signed transactions for the in-app purchase based on the order ID. Use the decoded transaction, JWSTransactionDecodedPayload, to identify information such as the `productId` and `purchaseDate` that you can use to provide customer support.

A response with an OrderLookupStatus value of `1` doesn’t contain a signed transactions array.

The App Store Server API returns information based on the customer’s in-app purchase history regardless of whether the customer installed, removed, or reinstalled the app on their devices.

## Topics

### Request data types

type orderId

The customer’s order ID from an App Store receipt for in-app purchases.

## See Also

### Order ID lookup

type orderId

The customer’s order ID from an App Store receipt for in-app purchases.

object OrderLookupResponse

A response that includes the order lookup status and an array of signed transactions for the in-app purchases in the order.

