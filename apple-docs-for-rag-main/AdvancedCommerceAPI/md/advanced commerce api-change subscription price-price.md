

- Advanced Commerce API
-  Change Subscription Price 

Web Service Endpoint

# Change Subscription Price

Increase or decrease the price of an auto-renewable subscription, a bundle, or individual items within a subscription at the next renewal.

Advanced Commerce API 1.0+

## URL

``` source
POST https://api.storekit.itunes.apple.com/advancedCommerce/v1/subscription/changePrice/{transactionId}
```

## Sandbox URL

``` source
POST https://api.storekit-sandbox.itunes.apple.com/advancedCommerce/v1/subscription/changePrice/{transactionId}
```

## Path Parameters

`transactionId`

`string`

 (Required) 

A transaction identifier of the auto-renewable subscription that is subject to the price change. Use the subscription’s original transaction ID or any subsequent transaction ID of a transaction related to the subscription.

## HTTP Body

SubscriptionPriceChangeRequest

The request body that contains the details of the price change.

Content-Type: application/json

## Response Codes

` 200 ``OK`

SubscriptionPriceChangeResponse

`OK`

Success

Content-Type: application/json

` 400 ``Bad Request`

`(`NullRequestInfoError` | `NullItemsError` | `NullSKUError` | `InvalidAppAccountTokenError` | `NullRequestReferenceIDError` | `InvalidRequestReferenceIDError` | `InvalidConsistencyTokenError` | `InvalidStorefrontError` | `InvalidCurrencyError` | `NegativePriceError` | `SKULengthExceededError` | `DescriptionLengthExceededError` | `DisplayNameLengthExceededError` | `InvalidProductError` | `InvalidSKUError` | `MismatchedStorefrontError` | `MissingPricingConfigForStorefrontError` | `OperationNotAllowedError` | `MalformedPayloadError`)`

`Bad Request`

Content-Type: application/json

` 401 ``Unauthorized`

`Unauthorized`

` 403 ``Forbidden`

`(`SubscriptionDoesNotExistError` | `SubscriptionNotEligibleError`)`

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

Handling subscription price changes

Identifying rate limits for Advanced Commerce APIs

Authorizing API requests from your server

## Discussion

Call this endpoint as the final step in changing the price of a subscription or any bundle or item within it. Based on the type of price change, you might need to communicate the change to customers or get their consent. For information about the communication requirements including their timing, see Handling subscription price changes.

Only active subscriptions that aren’t in a billing retry state are eligible for price changes. When you call this endpoint, the price change takes effect at the next subscription renewal. Call the endpoint no later than 24 hours before the renewal date to have it take effect at the renewal.

For information about providing prices, see Specifying prices for Advanced Commerce SKUs.

### Inform customers and get consent if needed

Determine whether you need to communicate a price change to the customer, as follows:

- Decreasing the price doesn’t require any communications with the customer. You can call this endpoint anytime you want to decrease prices.

- Increasing subscription prices requires you to notify the customer in advance. Some price increases also require you to obtain the customer’s consent. To determine whether you need price consent and for information about customer communications and their timing, see Handling subscription price changes.

Important

You need to communicate price increases to your customer, including through email, in-app messaging, and push notifications. To determine whether you need price consent and for information about customer communications and their timing, see Handling subscription price changes.

### Increase price of a SKU

If you’re increasing the price of any SKU associated with a subscription (such as the subscription itself, a bundle, or an individual item), follow these steps:

1.  Determine whether the price increase requires customer consent.

2.  If the increase doesn’t require customer consent, notify the customer of the price increase in advance, as described in Handling subscription price changes. Then, call this endpoint after you notify the customer.

3.  If the increase requires customer consent, call this endpoint only if you’ve obtained the customer’s consent. If you don’t obtain the customer’s consent to increase the price, don’t call this endpoint, and preserve the existing price.

## See Also

### Subscription price change from the server

object SubscriptionPriceChangeRequest

The request body you use to change the price of an auto-renewable subscription.

object SubscriptionPriceChangeResponse

A response that contains signed JWS renewal and JWS transaction information after a subscription price change request.

