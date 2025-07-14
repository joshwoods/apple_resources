

- MapKit
- MKMapView
- MKMapView.CameraBoundary
-  region 

Instance Property

# region

The coordinate region that describes the camera boundary.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
var region: MKCoordinateRegion { get }
```

## Discussion

Both the mapRect and the region represent the same camera boundary.

## See Also

### Accessing the boundary

var mapRect: MKMapRect

The map rectangle that describes the camera boundary.

