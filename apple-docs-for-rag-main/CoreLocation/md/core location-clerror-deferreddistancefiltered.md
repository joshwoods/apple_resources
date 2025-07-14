

- Core Location
- CLError
-  deferredDistanceFiltered 

Type Property

# deferredDistanceFiltered

A constant that indicates deferred mode doesn’t support distance filters.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var deferredDistanceFiltered: CLError.Code { get }
```

## Discussion

Set the distance filter to kCLDistanceFilterNone.

## See Also

### Getting deferred location update errors

static var deferredFailed: CLError.Code

A constant that indicates the location manager didn’t enter deferred mode for an unknown reason.

static var deferredCanceled: CLError.Code

A constant that indicates your app or the location manager canceled the request for deferred updates.

static var deferredAccuracyTooLow: CLError.Code

A constant that indicates deferred mode isn’t supported for the requested accuracy.

static var deferredNotUpdatingLocation: CLError.Code

A constant that indicates the location manager didn’t enter deferred mode because location updates were already disabled or paused.

