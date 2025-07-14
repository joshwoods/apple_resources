

- MapKit
- MKMapCamera
-  pitch 

Instance Property

# pitch

The viewing angle of the camera, in degrees.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
var pitch: CGFloat { get set }
```

## Discussion

A value of `0` results in a camera that points straight down at the map. Angles greater than `0` result in a camera that pitches toward the horizon by the specified number of degrees. If the map type is MKMapType.satellite or MKMapType.hybrid, the object clamps the pitch value to `0`.

The class may clamp the value in this property to a maximum value to maintain map readability. There’s no fixed maximum value, though, because the actual maximum value is dependent on the altitude of the camera.

## See Also

### Configuring the viewing angle

var centerCoordinate: CLLocationCoordinate2D

The map coordinate at the center of the map view.

var heading: CLLocationDirection

The heading of the camera (in degrees) relative to true north.

var centerCoordinateDistance: CLLocationDistance

The distance from the center point of the map to the camera, in meters.

var altitude: CLLocationDistance

The altitude above the ground, in meters.

Deprecated

