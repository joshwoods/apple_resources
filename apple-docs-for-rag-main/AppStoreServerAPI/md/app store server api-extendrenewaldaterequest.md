

- App Store Server API
-  ExtendRenewalDateRequest 

Object

# ExtendRenewalDateRequest

The request body that contains subscription-renewal-extension data for an individual subscription.

App Store Server API 1.1+

``` source
object ExtendRenewalDateRequest
```

## Properties

`extendByDays`

extendByDays

**Required**. The number of days to extend the subscription renewal date.

Maximum: `90`

`extendReasonCode`

extendReasonCode

**Required**. The reason code for the subscription date extension.

`requestIdentifier`

requestIdentifier

**Required**. A string that contains a value you provide to uniquely identify this renewal-date extension request.

Maximum length: `128`

## Discussion

Use this object with the Extend a Subscription Renewal Date endpoint.

## Topics

### Request data types

type extendByDays

The number of days to extend the subscription renewal date.

type extendReasonCode

The code that represents the reason for the subscription-renewal-date extension.

type requestIdentifier

A string that contains a unique identifier you provide to track each subscription-renewal-date extension request.

## See Also

### Subscription-renewal-date extension

Extending the renewal date for auto-renewable subscriptions

Compensate eligible active subscribers for service interruptions by extending a subscription’s renewal date.

Extend a Subscription Renewal Date

Extends the renewal date of a customer’s active subscription using the original transaction identifier.

Extend Subscription Renewal Dates for All Active Subscribers

Uses a subscription’s product identifier to extend the renewal date for all of its eligible active subscribers.

Get Status of Subscription Renewal Date Extensions

Checks whether a renewal date extension request completed, and provides the final count of successful or failed extensions.

object ExtendRenewalDateResponse

A response that indicates whether an individual renewal-date extension succeeded, and related details.

object MassExtendRenewalDateRequest

The request body that contains subscription-renewal-extension data to apply for all eligible active subscribers.

object MassExtendRenewalDateResponse

A response that indicates the server successfully received the subscription-renewal-date extension request.

object MassExtendRenewalDateStatusResponse

A response that indicates the current status of a request to extend the subscription renewal date to all eligible subscribers.

