

- MapKit
- MKMapView
-  mapType Deprecated

Instance Property

# mapType

The type of data the map view displays.

iOS 3.0–18.4DeprecatediPadOS 3.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.9–15.4DeprecatedtvOS 9.2+visionOS 1.0–2.4Deprecated

``` source
@MainActor
var mapType: MKMapType { get set }
```

Deprecated

Use the map view’s preferredConfiguration property with an MKMapConfiguration subclass to specify how the framework presents the map instead.

## Discussion

Changing the value in this property may cause the receiver to begin loading new map content. For example, changing from MKMapType.standard to MKMapType.satellite might cause it to begin loading the satellite imagery for the map. If the map needs new data, however, it loads asynchronously and MapKit sends appropriate messages to the receiver’s delegate indicating the status of the operation.

## See Also

### Related Documentation

Location and Maps Programming Guide

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

var isRotateEnabled: Bool

A Boolean value that indicates whether the map uses the camera’s heading information.

