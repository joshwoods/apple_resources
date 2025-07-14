

- App Store Server API
-  failedCount 

Type

# failedCount

The count of subscriptions that fail to receive a subscription-renewal-date extension.

App Store Server API 1.7+

``` source
int64 failedCount
```

## Discussion

For information about retrying a renewal date extension when if fails, see Extending the renewal date for auto-renewable subscriptions.

## See Also

### Data types

type complete

A Boolean value that indicates whether the App Store completed the request to extend a subscription renewal date to active subscribers.

type completeDate

The UNIX time, in milliseconds, that the App Store completes a request to extend a subscription renewal date for eligible subscribers.

type succeededCount

The count of subscriptions that successfully receive a subscription-renewal-date extension.

