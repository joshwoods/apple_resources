

- MapKit
- MKMapCamera
-  altitude Deprecated

Instance Property

# altitude

The altitude above the ground, in meters.

iOS 7.0–18.4DeprecatediPadOS 7.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.9–15.4DeprecatedtvOS 9.2+visionOS 1.0–2.4Deprecated

``` source
var altitude: CLLocationDistance { get set }
```

Deprecated

Use centerCoordinateDistance instead.

## Discussion

The value you specify for this property can’t be less than `0`.

Changing this property may also change the maximum pitch for the map. If the current pitch value exceeds the new maximum, the class clamps the pitch property to the new maximum.

## See Also

### Configuring the viewing angle

var centerCoordinate: CLLocationCoordinate2D

The map coordinate at the center of the map view.

var heading: CLLocationDirection

The heading of the camera (in degrees) relative to true north.

var centerCoordinateDistance: CLLocationDistance

The distance from the center point of the map to the camera, in meters.

var pitch: CGFloat

The viewing angle of the camera, in degrees.

