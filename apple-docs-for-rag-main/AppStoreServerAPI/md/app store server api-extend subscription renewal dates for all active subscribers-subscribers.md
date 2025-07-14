

- App Store Server API
-  Extend Subscription Renewal Dates for All Active Subscribers 

Web Service Endpoint

# Extend Subscription Renewal Dates for All Active Subscribers

Uses a subscription’s product identifier to extend the renewal date for all of its eligible active subscribers.

App Store Server API 1.7+

## URL

``` source
POST https://api.storekit.itunes.apple.com/inApps/v1/subscriptions/extend/mass
```

## Sandbox URL

``` source
POST https://api.storekit-sandbox.itunes.apple.com/inApps/v1/subscriptions/extend/mass
```

## HTTP Body

MassExtendRenewalDateRequest

The request body for extending a subscription renewal date for all of its active subscribers.

Content-Type: application/json

## Response Codes

` 200 ``OK`

MassExtendRenewalDateResponse

`OK`

Request succeeded.

If you reuse the requestIdentifier to call the endpoint again, the server responds with `200`.

Content-Type: application/json

` 400 ``Bad Request`

`(`InvalidExtendByDaysError` | `InvalidProductIdError` | `InvalidExtendReasonCodeError` | `InvalidRequestIdentifierError` | `InvalidEmptyStorefrontCountryCodeListError` | `InvalidStorefrontCountryCodeError`)`

`Bad Request`

The request is invalid and can’t be accepted.

Content-Type: application/json

` 401 ``Unauthorized`

`Unauthorized`

The JSON Web Token (JWT) in the authorization header is invalid. For more information, see Generating JSON Web Tokens for API requests.

` 403 ``Forbidden`

`(`SubscriptionExtensionIneligibleError` | `SubscriptionMaxExtensionError`)`

`Forbidden`

The request is invalid and can’t be accepted.

Content-Type: application/json

` 404 ``Not Found`

StatusRequestNotFoundError

`Not Found`

The server didn’t find a subscription-renewal-date extension request for the request identifier and product identifier you provided.

Content-Type: application/json

` 429 `

RateLimitExceededError

The request exceeded the rate limit.

Content-Type: application/json

` 500 ``Internal Server Error`

`(`GeneralInternalError` | `GeneralInternalRetryableError`)`

`Internal Server Error`

The request failed. This may be due to a temporary outage. Check the specific error message for further information.

Content-Type: application/json

## Mentioned in 

Extending the renewal date for auto-renewable subscriptions

Identifying rate limits

App Store Server API changelog

## Discussion

Use this endpoint to compensate your customers for temporary service outages, canceled events, or interruptions to live streamed events by extending the renewal date of their paid, active subscription. This endpoint acts on all active subscriptions for the product identifier you specify, and is limited to the storefronts you optionally specify.

To call this endpoint, provide the subscription product identifier that experienced the service interruption, and other information, in the request body, MassExtendRenewalDateRequest.

A successful response with an `HTTP 200` status code contains the MassExtendRenewalDateResponse object, which includes the same unique `requestIdentifier` you provide in the request. This endpoint is an asynchronous request. A successful response indicates that the App Store server is processing the request. Status codes other than `HTTP 200` indicate that the request failed.

Note

After the subscription renewal extension goes into effect, there’s no way to reverse it. The extension period doesn’t count toward the one year of paid service when the App Store calculates the developer’s commission rate.

After a successful renewal date extension, Apple sends an email to notify the customer of their updated subscription renewal date.

For more information about this endpoint, including subscription eligibility, getting status notifications, and retrying extensions that fail, see Extending the renewal date for auto-renewable subscriptions.

## See Also

### Subscription-renewal-date extension

Extending the renewal date for auto-renewable subscriptions

Compensate eligible active subscribers for service interruptions by extending a subscription’s renewal date.

Extend a Subscription Renewal Date

Extends the renewal date of a customer’s active subscription using the original transaction identifier.

Get Status of Subscription Renewal Date Extensions

Checks whether a renewal date extension request completed, and provides the final count of successful or failed extensions.

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

