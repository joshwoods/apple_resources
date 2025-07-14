

- App Store Server API
-  MassExtendRenewalDateStatusResponse 

Object

# MassExtendRenewalDateStatusResponse

A response that indicates the current status of a request to extend the subscription renewal date to all eligible subscribers.

App Store Server API 1.7+

``` source
object MassExtendRenewalDateStatusResponse
```

## Properties

`requestIdentifier`

requestIdentifier

The `UUID` that represents your request for a subscription-renewal-date extension.

Maximum length: `128`

`complete`

complete

A Boolean value that’s `TRUE` to indicate that the App Store completed your request to extend a subscription renewal date for all eligible subscribers.

The value is `FALSE` if the request is in progress.

`completeDate`

completeDate

The date that the App Store completes the request.

Appears only if `complete` is `TRUE`.

`failedCount`

failedCount

The final count of subscribers that fail to receive a subscription-renewal-date extension.

Appears only if `complete` is `TRUE`.

`succeededCount`

succeededCount

The final count of subscribers that successfully receive a subscription-renewal-date extension.

Appears only if `complete` is `TRUE`.

## Mentioned in 

App Store Server API changelog

## Discussion

The App Store server sends this response when you call the Get Status of Subscription Renewal Date Extensions endpoint. Your request to Extend Subscription Renewal Dates for All Active Subscribers is complete when the value of the `complete` field is `TRUE`. Otherwise, the request is still in progress.

The App Store server also sends real-time notifications as it’s processing the subscription-renewal-date extension, including notifications with notificationType values of `RENEWAL_EXTENSION` and `RENEWAL_EXTENDED`. For more information, see App Store Server Notifications. For more information about extending subscription renewal dates, see Extending the renewal date for auto-renewable subscriptions.

## Topics

### Data types

type complete

A Boolean value that indicates whether the App Store completed the request to extend a subscription renewal date to active subscribers.

type completeDate

The UNIX time, in milliseconds, that the App Store completes a request to extend a subscription renewal date for eligible subscribers.

type failedCount

The count of subscriptions that fail to receive a subscription-renewal-date extension.

type succeededCount

The count of subscriptions that successfully receive a subscription-renewal-date extension.

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

object ExtendRenewalDateRequest

The request body that contains subscription-renewal-extension data for an individual subscription.

object ExtendRenewalDateResponse

A response that indicates whether an individual renewal-date extension succeeded, and related details.

object MassExtendRenewalDateRequest

The request body that contains subscription-renewal-extension data to apply for all eligible active subscribers.

object MassExtendRenewalDateResponse

A response that indicates the server successfully received the subscription-renewal-date extension request.

