

- App Store Server API
-  Get Status of Subscription Renewal Date Extensions 

Web Service Endpoint

# Get Status of Subscription Renewal Date Extensions

Checks whether a renewal date extension request completed, and provides the final count of successful or failed extensions.

App Store Server API 1.7+

## URL

``` source
GET https://api.storekit.itunes.apple.com/inApps/v1/subscriptions/extend/mass/{productId}/{requestIdentifier}
```

## Sandbox URL

``` source
GET https://api.storekit-sandbox.itunes.apple.com/inApps/v1/subscriptions/extend/mass/{productId}/{requestIdentifier}
```

## Path Parameters

`productId`

productId

 (Required) 

The product identifier of the auto-renewable subscription that you request a renewal-date extension for.

`requestIdentifier`

requestIdentifier

 (Required) 

The `UUID` that represents your request to the Extend Subscription Renewal Dates for All Active Subscribers endpoint.

Maximum length: `128`

## Response Codes

` 200 ``OK`

MassExtendRenewalDateStatusResponse

`OK`

The request succeeded.

Content-Type: application/json

` 400 ``Bad Request`

`(`InvalidProductIdError` | `InvalidRequestIdentifierError`)`

`Bad Request`

The request is invalid.

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

Extending the renewal date for auto-renewable subscriptions

## Discussion

This endpoint provides basic status information about a request you initiate when you call the Extend Subscription Renewal Dates for All Active Subscribers endpoint. Such requests may take hours, or even days, depending on the number of subscribers. This status tells whether the request is complete. If so, it has the total count of successful and failed subscription-renewal-date extensions.

Tip

If you don’t need this status on demand, or need more details, use the App Store Server Notifications for near real-time status information instead. For more information about related notifications, see Extending the renewal date for auto-renewable subscriptions.

## See Also

### Subscription-renewal-date extension

Extending the renewal date for auto-renewable subscriptions

Compensate eligible active subscribers for service interruptions by extending a subscription’s renewal date.

Extend a Subscription Renewal Date

Extends the renewal date of a customer’s active subscription using the original transaction identifier.

Extend Subscription Renewal Dates for All Active Subscribers

Uses a subscription’s product identifier to extend the renewal date for all of its eligible active subscribers.

object ExtendRenewalDateRequest

The request body that contains subscription-renewal-extension data for an individual subscription.

object ExtendRenewalDateResponse

A response that indicates whether an individual renewal-date extension succeeded, and related details.

object MassExtendRenewalDateRequest

The request body that contains subscription-renewal-extension data to apply for all eligible active subscribers.

object MassExtendRenewalDateResponse

A response that indicates the server successfully received the subscription-renewal-date extension request.

object MassExtendRenewalDateStatusResponse

A response that indicates the current status of a request to extend the subscription renewal date to all eligible subscribers.

