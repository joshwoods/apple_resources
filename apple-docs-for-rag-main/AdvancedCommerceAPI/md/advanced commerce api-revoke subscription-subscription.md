

- Advanced Commerce API
-  Revoke Subscription 

Web Service Endpoint

# Revoke Subscription

Immediately cancel a customer’s subscription and all the items that are included in the subscription, and request a full or prorated refund.

Advanced Commerce API 1.0+

## URL

``` source
POST https://api.storekit.itunes.apple.com/advancedCommerce/v1/subscription/revoke/{transactionId}
```

## Sandbox URL

``` source
POST https://api.storekit-sandbox.itunes.apple.com/advancedCommerce/v1/subscription/revoke/{transactionId}
```

## Path Parameters

`transactionId`

`string`

 (Required) 

The transaction identifier of the auto-renewable subscription to revoke. Use the subscription’s original transaction ID or any subsequent transaction ID of a transaction related to the subscription.

## HTTP Body

SubscriptionRevokeRequest

Content-Type: application/json

## Response Codes

` 200 ``OK`

SubscriptionRevokeResponse

`OK`

Request succeeded.

Content-Type: application/json

` 400 ``Bad Request`

`(`RepeatedRequestReferenceIdError` | `NullRequestInfoError` | `InvalidAppAccountTokenError` | `NullRequestReferenceIDError` | `InvalidRequestReferenceIDError` | `InvalidConsistencyTokenError` | `InvalidStorefrontError` | `MismatchedStorefrontError` | `MismatchedStorefrontError` | `OperationNotAllowedError` | `MalformedPayloadError` | `SimulateRefundDeclineOnlyInSandboxError` | `RefundAmountWithoutCustomError` | `NullRefundRiskingError` | `InvalidRefundTypeError` | `InvalidRefundReasonError` | `NegativeRefundAmountError` | `NullRefundAmountError` | `NullRefundReasonError` | `NullRefundTypeError` | `PendingRefundError` | `RevokeOnInactiveSubscriptionError`)`

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

Identifying rate limits for Advanced Commerce APIs

Authorizing API requests from your server

Advanced Commerce API changelog

## Discussion

When this endpoint succeeds, the system sets the subscription’s auto-renew status to `false`, and revokes the subscription with a full or prorated refund. The App Store Server Notifications sends a `REFUND` notificationType to your App Store Server Notifications V2 endpoint. Check the `revocationDate` property in the notification’s JWSTransactionDecodedPayload. Turn off service for the subscription and its items as of the revocation date. Don’t turn off service to the subscription until you receive the notification.

To cancel a subscription at the end of the current period instead, see Cancel a Subscription.

Note

To use the `Revoke Subscription` endpoint, your membership Account Holder must sign the Advanced Commerce API Addendum, and you must meet certain eligibility requirements. For more information, see Advanced Commerce API. If the most recent version of this agreement isn’t yet accepted, you can’t call this endpoint, and it returns an error.

Refer to the Advanced Commerce API Addendum to learn the use cases for the Cancel a Subscription, `Revoke Subscription`, and Request Transaction Refund APIs.

## See Also

### Subscription revocation from the server

object SubscriptionRevokeRequest

The request body you provide to terminate a subscription and all its items immediately.

object SubscriptionRevokeResponse

The response body for a successful revoke-subscription request.

