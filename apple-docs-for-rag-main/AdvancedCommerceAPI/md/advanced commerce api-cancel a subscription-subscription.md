

- Advanced Commerce API
-  Cancel a Subscription 

Web Service Endpoint

# Cancel a Subscription

Turn off automatic renewal to cancel a customer’s auto-renewable subscription.

Advanced Commerce API 1.0+

## URL

``` source
POST https://api.storekit.itunes.apple.com/advancedCommerce/v1/subscription/cancel/{transactionId}
```

## Sandbox URL

``` source
POST https://api.storekit-sandbox.itunes.apple.com/advancedCommerce/v1/subscription/cancel/{transactionId}
```

## Path Parameters

`transactionId`

`string`

 (Required) 

The transaction identifier of the auto-renewable subscription to cancel.

## HTTP Body

SubscriptionCancelRequest

The request body that includes information about the subscription to cancel.

Content-Type: application/json

## Response Codes

` 200 ``OK`

SubscriptionCancelResponse

`OK`

Success

Content-Type: application/json

` 400 ``Bad Request`

`(`NullRequestInfoError` | `InvalidAppAccountTokenError` | `NullRequestReferenceIDError` | `InvalidRequestReferenceIDError` | `InvalidConsistencyTokenError` | `InvalidStorefrontError` | `MismatchedStorefrontError` | `OperationNotAllowedError` | `MalformedPayloadError`)`

`Bad Request`

Content-Type: application/json

` 401 ``Unauthorized`

`Unauthorized`

` 403 ``Forbidden`

`(`SubscriptionDoesNotExistError` | `SubscriptionNotEligibleError` | `ProductNotOwnedError`)`

`Forbidden`

Content-Type: application/json

` 404 ``Not Found`

TransactionIdNotFoundError

`Not Found`

Content-Type: application/json

` 429 `

RateLimitExceededError

Content-Type: application/json

` 500 ``Internal Server Error`

`(`GeneralInternalError` | `GeneralInternalRetryableError`)`

`Internal Server Error`

Content-Type: application/json

## Mentioned in 

Authorizing API requests from your server

Identifying rate limits for Advanced Commerce APIs

## Discussion

When this endpoint succeeds, the system sets the subscription’s auto-renew status to `false` and the subscription doesn’t renew at the next renewal period. The customer continues to have access to the subscription until the end of the current period.

To immediately cancel a subscription instead, see Revoke Subscription.

Note

To use the `Cancel a Subscription` endpoint, your membership Account Holder must sign the Advanced Commerce API Addendum, and you must meet certain eligibility requirements. For more information, see Advanced Commerce API. If the most recent version of this agreement isn’t yet accepted, you can’t call this endpoint, and it returns an error.

Refer to the Advanced Commerce API Addendum to learn the use cases for the `Cancel a Subscription`, Revoke Subscription, and Request Transaction Refund APIs.

## See Also

### Subscription cancellation from the server

object SubscriptionCancelRequest

The request body for turning off automatic renewal of a subscription.

object SubscriptionCancelResponse

The response body for a successful subscription cancellation.

