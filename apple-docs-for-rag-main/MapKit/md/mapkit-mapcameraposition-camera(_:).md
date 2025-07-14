

- MapKit
- MapCameraPosition
-  camera(\_:) 

Type Method

# camera(\_:)

Creates a new camera position from an existing map camera you provide.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
static func camera(_ camera: MapCamera) -> MapCameraPosition
```

## Parameters 

`camera`  

The map camera to convert.

## Return Value

Returns a new camera position.

## See Also

### Creating a camera position

static func item(MKMapItem, allowsAutomaticPitch: Bool) -> MapCameraPosition

Creates a new camera position centered on a map item and automatic pitch selection you provide.

static func rect(MKMapRect) -> MapCameraPosition

Creates a new camera position with the map boundaries you provide.

static func region(MKCoordinateRegion) -> MapCameraPosition

Creates a new camera position the coordinate region you provide.

static func userLocation(followsHeading: Bool, fallback: MapCameraPosition) -> MapCameraPosition

Creates a camera position with the specific fallback position and optionally follows the user’s heading.

