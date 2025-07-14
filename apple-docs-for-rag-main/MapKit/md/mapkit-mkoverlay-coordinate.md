

- MapKit
- MKOverlay
-  coordinate 

Instance Property

# coordinate

The approximate center point of the overlay area.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
var coordinate: CLLocationCoordinate2D { get }
```

**Required**

## Discussion

This point is typically set to the center point of the map’s bounding rectangle. The overlay uses it as the anchor point for any callouts that display for the annotation.

## See Also

### Related Documentation

Location and Maps Programming Guide

### Describing the overlay geometry

var boundingMapRect: MKMapRect

The projected rectangle that encompasses the overlay.

**Required**

