

- MapKit
- MKMapView
- MKMapView.CameraBoundary
-  mapRect 

Instance Property

# mapRect

The map rectangle that describes the camera boundary.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
var mapRect: MKMapRect { get }
```

## Discussion

Both the mapRect and the region represent the same camera boundary.

## See Also

### Accessing the boundary

var region: MKCoordinateRegion

The coordinate region that describes the camera boundary.

