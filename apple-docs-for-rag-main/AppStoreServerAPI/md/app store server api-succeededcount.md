

- App Store Server API
-  succeededCount 

Type

# succeededCount

The count of subscriptions that successfully receive a subscription-renewal-date extension.

App Store Server API 1.7+

``` source
int64 succeededCount
```

## Discussion

For information about a subscription’s eligibility to receive a subscription-renewal-date extension, see Extending the renewal date for auto-renewable subscriptions.

## See Also

### Data types

type complete

A Boolean value that indicates whether the App Store completed the request to extend a subscription renewal date to active subscribers.

type completeDate

The UNIX time, in milliseconds, that the App Store completes a request to extend a subscription renewal date for eligible subscribers.

type failedCount

The count of subscriptions that fail to receive a subscription-renewal-date extension.

