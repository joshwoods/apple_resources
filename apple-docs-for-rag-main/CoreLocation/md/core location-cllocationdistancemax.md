

- Core Location
-  CLLocationDistanceMax 

Global Variable

# CLLocationDistanceMax

A constant indicating the maximum distance.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.14+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let CLLocationDistanceMax: CLLocationDistance
```

## Discussion

When scheduling deferred updates, you can use this constant to indicate that a new update should be triggered only after the device moves a significantly large distance.

## See Also

### Specifying distance and accuracy

var distanceFilter: CLLocationDistance

The minimum distance in meters the device must move horizontally before an update event is generated.

let kCLDistanceFilterNone: CLLocationDistance

A constant indicating that all movement should be reported.

typealias CLLocationDistance

A distance in meters from an existing location.

var desiredAccuracy: CLLocationAccuracy

The accuracy of the location data that your app wants to receive.

typealias CLLocationAccuracy

The accuracy of a geographical coordinate.

