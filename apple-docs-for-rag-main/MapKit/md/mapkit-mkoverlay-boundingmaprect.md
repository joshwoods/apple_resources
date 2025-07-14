

- MapKit
- MKOverlay
-  boundingMapRect 

Instance Property

# boundingMapRect

The projected rectangle that encompasses the overlay.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
var boundingMapRect: MKMapRect { get }
```

**Required**

## Discussion

This property contains the smallest rectangle that completely encompasses the overlay. Implementers of this protocol need to set this area when implementing their overlay class, and after setting it, not change it. Specify the rectangle using projected coordinates — that is, coordinates you obtain by projecting the globe onto a two-dimensional surface.

## See Also

### Describing the overlay geometry

var coordinate: CLLocationCoordinate2D

The approximate center point of the overlay area.

**Required**

