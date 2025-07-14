

- Advanced Commerce API
-  Request Transaction Refund 

Web Service Endpoint

# Request Transaction Refund

Request a refund for a one-time charge or subscription transaction.

Advanced Commerce API 1.0+

## URL

``` source
POST https://api.storekit.itunes.apple.com/advancedCommerce/v1/transaction/requestRefund/{transactionId}
```

## Sandbox URL

``` source
POST https://api.storekit-sandbox.itunes.apple.com/advancedCommerce/v1/transaction/requestRefund/{transactionId}
```

## Path Parameters

`transactionId`

`string`

 (Required) 

The transaction identifier for which you request a refund.

## HTTP Body

RequestRefundRequest

The request body.

Content-Type: application/json

## Response Codes

` 200 ``OK`

RequestRefundResponse

`OK`

Request succeeded.

Content-Type: application/json

` 400 ``Bad Request`

`(`RepeatedRequestReferenceIdError` | `NullRequestInfoError` | `InvalidAppAccountTokenError` | `NullRequestReferenceIDError` | `InvalidRequestReferenceIDError` | `InvalidConsistencyTokenError` | `InvalidStorefrontError` | `MismatchedStorefrontError` | `MismatchedStorefrontError` | `OperationNotAllowedError` | `MalformedPayloadError` | `SimulateRefundDeclineOnlyInSandboxError` | `RefundAmountWithoutCustomError` | `NullRefundRiskingError` | `InvalidRefundTypeError` | `InvalidRefundReasonError` | `NegativeRefundAmountError` | `NullRefundAmountError` | `NullRefundReasonError` | `NullRefundTypeError` | `RemovalAllNotAllowedError` | `PendingRefundError` | `ProratedOnlyLatestTransactionError` | `PartialSimulateRefundDeclineError`)`

`Bad Request`

Content-Type: application/json

` 401 ``Unauthorized`

`Unauthorized`

The JSON Web Token (JWT) in the authorization header is invalid. For more information, see Authorizing API requests from your server.

` 403 ``Forbidden`

`(`SubscriptionDoesNotExistError` | `SubscriptionNotEligibleError` | `ProductNotOwnedError` | `InsufficientFundsError` | `AlreadyRefundedError` | `TransactionNotRefundableError`)`

`Forbidden`

Content-Type: application/json

` 404 ``Not Found`

TransactionIdNotFoundError

`Not Found`

Content-Type: application/json

` 429 `

RateLimitExceededError

The request exceeded the rate limit. For more information, see Identifying rate limits for Advanced Commerce APIs.

Content-Type: application/json

` 500 ``Internal Server Error`

`(`GeneralInternalError` | `GeneralInternalRetryableError`)`

`Internal Server Error`

Server error. Try again later.

Content-Type: application/json

## Mentioned in 

Authorizing API requests from your server

Identifying rate limits for Advanced Commerce APIs

Advanced Commerce API changelog

## Discussion

Note

To use the `Request Transaction Refund` endpoint, your membership Account Holder must sign the Advanced Commerce API Addendum, and you must meet certain eligibility requirements. For more information, see Advanced Commerce API. If the most recent version of this agreement isn’t yet accepted, you can’t call this endpoint, and it returns an error.

Refer to the Advanced Commerce API Addendum to learn the use cases for the Cancel a Subscription, Revoke Subscription, and `Request Transaction Refund` APIs.

## See Also

### Refund request from the server

object RequestRefundRequest

The request body for requesting a refund for a transaction.

object RequestRefundResponse

The response body for a transaction refund request.

object RequestRefundItem

Information about the refund request for an item, such as its SKU, the refund amount, reason, and type.

