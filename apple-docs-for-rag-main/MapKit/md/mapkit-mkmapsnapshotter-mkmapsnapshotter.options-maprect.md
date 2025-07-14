

- MapKit
- MKMapSnapshotter
- MKMapSnapshotter.Options
-  mapRect 

Instance Property

# mapRect

The map rectangle that you want to capture.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
var mapRect: MKMapRect { get set }
```

## Discussion

Use this property to specify the map using map view points. If you assign a value for this property, the snapshotter updates the value in the region property to match the corresponding map rectangle as closely as possible.

The snapshotter sets the default value of this property to a map rectangle that encompasses the user’s country or region, based on the current locale information.

## See Also

### Configuring the snapshot region

var region: MKCoordinateRegion

The area of the map that you want to capture.

var camera: MKMapCamera

The camera to use when taking the map snapshot.

