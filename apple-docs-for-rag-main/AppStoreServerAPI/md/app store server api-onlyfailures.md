

- App Store Server API
-  onlyFailures 

Type

# onlyFailures

A Boolean value that indicates whether the response includes only notifications that failed to reach your server.

App Store Server API 1.8+

``` source
boolean onlyFailures
```

## Mentioned in 

App Store Server API changelog

## Discussion

A value of `true` indicates that you want to receive just the App Store server notifications that failed to reach your server, including those that the App Store server is currently retrying.

## See Also

### Data types

type startDate

The start date of a timespan, expressed in UNIX time, in milliseconds.

type endDate

The end date of a timespan, expressed in UNIX time, in milliseconds.

type notificationType

A notification type value that App Store Server Notifications 2 uses.

type notificationSubtype

A notification subtype value that App Store Server Notifications 2 uses.

