

- MapKit
- MapCameraPosition
-  positionedByUser 

Instance Property

# positionedByUser

A Boolean value that indicates whether the person specified the camera position by interacting with the map.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
var positionedByUser: Bool { get }
```

## See Also

### Information about camera position and framing

static var automatic: MapCameraPosition

The position that frames the map’s content.

var allowsAutomaticPitch: Bool

The setting that allows the map’s camera to automatically set the pitch when framing the item.

var camera: MapCamera?

A map camera that defines the camera positioning.

var fallbackPosition: MapCameraPosition?

The position to use if the framework hasn’t resolved the person’s location.

var item: MKMapItem?

The item the map is framing.

var rect: MKMapRect?

The position that frames the given map rectangle.

var region: MKCoordinateRegion?

The coordinate region to frame.

