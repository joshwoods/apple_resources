

- Core Location
- CLError
- CLError.Code
-  CLError.Code.deferredCanceled 

Case

# CLError.Code.deferredCanceled

A constant that indicates your app or the location manager canceled the request for deferred updates.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case deferredCanceled
```

## Discussion

This error is returned if you call the disallowDeferredLocationUpdates() method or schedule a new deferred update before the previous deferred update request is processed. The location manager may also report this error too. For example, if the app is in the foreground when a new location is determined, the location manager cancels deferred updates and delivers the location data to your app.

## See Also

### Getting deferred location update errors

case deferredFailed

A constant that indicates the location manager didn’t enter deferred mode for an unknown reason.

case deferredAccuracyTooLow

A constant that indicates deferred mode isn’t supported for the requested accuracy.

case deferredDistanceFiltered

A constant that indicates deferred mode doesn’t support distance filters.

case deferredNotUpdatingLocation

A constant that indicates the location manager didn’t enter deferred mode because location updates were already disabled or paused.

