

- MapKit
- MKMapItem
-  forCurrentLocation() 

Type Method

# forCurrentLocation()

Creates and returns a singleton map item object representing the user’s location.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+watchOS 2.0+

``` source
class func forCurrentLocation() -> MKMapItem
```

## Return Value

An `MKMapItem` object representing the user’s location.

## Discussion

For privacy reasons, and because the user’s location can change, the map item that this method returns doesn’t contain any coordinate data. When you need the actual location of the user, use the Core Location framework to retrieve it.

## See Also

### Related Documentation

Location and Maps Programming Guide

### Creating map items

init(placemark: MKPlacemark)

Creates and returns a map item object using the specified placemark object.

