

- MapKit
- MKMapSnapshotter
- MKMapSnapshotter.Options
-  region 

Instance Property

# region

The area of the map that you want to capture.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
var region: MKCoordinateRegion { get set }
```

## Discussion

Use this property to specify the map using geographical coordinates. If you assign a value for this property, the snapshotter updates the value in the mapRect property to match the corresponding area as closely as possible.

The snapshotter sets the default value of this property to an area that encompasses the user’s country or region, based on the current locale information.

## See Also

### Configuring the snapshot region

var mapRect: MKMapRect

The map rectangle that you want to capture.

var camera: MKMapCamera

The camera to use when taking the map snapshot.

