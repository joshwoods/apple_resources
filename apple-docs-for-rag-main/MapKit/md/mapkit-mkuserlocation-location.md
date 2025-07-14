

- MapKit
- MKUserLocation
-  location 

Instance Property

# location

The location of the device.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
var location: CLLocation? { get }
```

## Mentioned in 

Converting a user’s location to a descriptive placemark

## Discussion

This property contains `nil` if the map view isn’t showing the user’s location, or if the map view is still determining the user’s location.

## See Also

### Related Documentation

Location and Maps Programming Guide

### Determining the user’s location

var isUpdating: Bool

A Boolean value that indicates whether the map view is updating the user’s location.

var heading: CLHeading?

The heading of the user’s location.

