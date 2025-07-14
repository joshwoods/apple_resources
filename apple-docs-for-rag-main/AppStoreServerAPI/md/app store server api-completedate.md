

- App Store Server API
-  completeDate 

Type

# completeDate

The UNIX time, in milliseconds, that the App Store completes a request to extend a subscription renewal date for eligible subscribers.

App Store Server API 1.7+

``` source
timestamp completeDate
```

## Discussion

For more information about a requesting a subscription-renewal-date extension, see Extend Subscription Renewal Dates for All Active Subscribers.

## See Also

### Data types

type complete

A Boolean value that indicates whether the App Store completed the request to extend a subscription renewal date to active subscribers.

type failedCount

The count of subscriptions that fail to receive a subscription-renewal-date extension.

type succeededCount

The count of subscriptions that successfully receive a subscription-renewal-date extension.

