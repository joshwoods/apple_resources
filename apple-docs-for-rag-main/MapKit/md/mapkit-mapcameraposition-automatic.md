

- MapKit
- MapCameraPosition
-  automatic 

Type Property

# automatic

The position that frames the map’s content.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
static var automatic: MapCameraPosition { get }
```

## See Also

### Information about camera position and framing

var allowsAutomaticPitch: Bool

The setting that allows the map’s camera to automatically set the pitch when framing the item.

var camera: MapCamera?

A map camera that defines the camera positioning.

var fallbackPosition: MapCameraPosition?

The position to use if the framework hasn’t resolved the person’s location.

var item: MKMapItem?

The item the map is framing.

var positionedByUser: Bool

A Boolean value that indicates whether the person specified the camera position by interacting with the map.

var rect: MKMapRect?

The position that frames the given map rectangle.

var region: MKCoordinateRegion?

The coordinate region to frame.

