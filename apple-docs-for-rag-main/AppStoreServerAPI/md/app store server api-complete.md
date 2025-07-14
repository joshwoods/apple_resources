

- App Store Server API
-  complete 

Type

# complete

A Boolean value that indicates whether the App Store completed the request to extend a subscription renewal date to active subscribers.

App Store Server API 1.7+

``` source
boolean complete
```

## Discussion

The request is complete when this value is `TRUE`. For more information about the subscription-renewal-date extension, see Extend Subscription Renewal Dates for All Active Subscribers.

## See Also

### Data types

type completeDate

The UNIX time, in milliseconds, that the App Store completes a request to extend a subscription renewal date for eligible subscribers.

type failedCount

The count of subscriptions that fail to receive a subscription-renewal-date extension.

type succeededCount

The count of subscriptions that successfully receive a subscription-renewal-date extension.

