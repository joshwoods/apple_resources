

- MapKit
- MKMapSnapshotter
- MKMapSnapshotter.Options
-  camera 

Instance Property

# camera

The camera to use when taking the map snapshot.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
@NSCopying
var camera: MKMapCamera { get set }
```

## Discussion

Specify a camera object if you want to change the pitch, altitude, or heading information applied to the map.

## See Also

### Configuring the snapshot region

var region: MKCoordinateRegion

The area of the map that you want to capture.

var mapRect: MKMapRect

The map rectangle that you want to capture.

