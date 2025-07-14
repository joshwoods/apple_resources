

- MapKit
- MKCircle
-  boundingMapRect 

Instance Property

# boundingMapRect

The bounding rectangle of the circular area.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
var boundingMapRect: MKMapRect { get }
```

## Discussion

As latitude values move away from the equator and toward the poles, the physical distance between map points gets smaller. This means that the map needs more map points to represent the same distance. As a result, the bounding rectangle of a circle overlay gets larger as the center point of that circle moves away from the equator and toward the poles.

## See Also

### Accessing the overlay’s attributes

var coordinate: CLLocationCoordinate2D

The center point of the circular area, specified as a latitude and longitude.

var radius: CLLocationDistance

The radius of the circular area, in meters.

