

- MapKit
- MKMapView
-  isRotateEnabled 

Instance Property

# isRotateEnabled

A Boolean value that indicates whether the map uses the camera’s heading information.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+visionOS 1.0+

``` source
@MainActor
var isRotateEnabled: Bool { get set }
```

## Discussion

When this property is true and the framework associates a valid camera with the map, the map uses the camera’s heading angle to rotate the plane of the map around its center point. When this property is false, the map view ignores the camera’s heading angle and the map orients so that the map view situates true north at the top.

## See Also

### Accessing map properties

enum MKMapType

The type of map to display.

Deprecated

var isZoomEnabled: Bool

A Boolean value that determines whether the user may use pinch gestures to zoom in and out of the map.

var isScrollEnabled: Bool

A Boolean value that determines whether the user may scroll around the map.

var isPitchEnabled: Bool

A Boolean value that indicates whether the map uses the camera’s pitch information.

var mapType: MKMapType

The type of data the map view displays.

Deprecated

