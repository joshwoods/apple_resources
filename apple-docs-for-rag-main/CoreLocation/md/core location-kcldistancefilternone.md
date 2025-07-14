

- Core Location
-  kCLDistanceFilterNone 

Global Variable

# kCLDistanceFilterNone

A constant indicating that all movement should be reported.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kCLDistanceFilterNone: CLLocationDistance
```

## Discussion

Use this constant to specify that any change in location should trigger a new location update.

## See Also

### Specifying distance and accuracy

var distanceFilter: CLLocationDistance

The minimum distance in meters the device must move horizontally before an update event is generated.

let CLLocationDistanceMax: CLLocationDistance

A constant indicating the maximum distance.

typealias CLLocationDistance

A distance in meters from an existing location.

var desiredAccuracy: CLLocationAccuracy

The accuracy of the location data that your app wants to receive.

typealias CLLocationAccuracy

The accuracy of a geographical coordinate.

