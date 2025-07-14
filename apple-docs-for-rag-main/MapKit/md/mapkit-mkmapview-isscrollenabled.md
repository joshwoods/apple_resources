

- MapKit
- MKMapView
-  isScrollEnabled 

Instance Property

# isScrollEnabled

A Boolean value that determines whether the user may scroll around the map.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
var isScrollEnabled: Bool { get set }
```

## Discussion

This property controls only user interactions with the map. If you set the value of this property to false, you may still change the map location programmatically by changing the value in the region property.

The default value of this property is true.

## See Also

### Accessing map properties

enum MKMapType

The type of map to display.

Deprecated

var isZoomEnabled: Bool

A Boolean value that determines whether the user may use pinch gestures to zoom in and out of the map.

var isPitchEnabled: Bool

A Boolean value that indicates whether the map uses the camera’s pitch information.

var isRotateEnabled: Bool

A Boolean value that indicates whether the map uses the camera’s heading information.

var mapType: MKMapType

The type of data the map view displays.

Deprecated

