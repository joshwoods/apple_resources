

- MapKit
- MKCircle
-  init(center:radius:) 

Initializer

# init(center:radius:)

Creates and returns a circle object using the specified coordinate and radius.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
convenience init(
    center coord: CLLocationCoordinate2D,
    radius: CLLocationDistance
)
```

## Parameters 

`coord`  

The center point of the circle, specified as a latitude and longitude value.

`radius`  

The radius of the circle, measured in meters from the center point.

## Return Value

A circle overlay object.

## See Also

### Related Documentation

Location and Maps Programming Guide

### Creating a circle overlay

convenience init(mapRect: MKMapRect)

Creates and returns a circle object that derives the circular area from the specified rectangle.

