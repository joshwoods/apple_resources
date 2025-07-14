

- MapKit
- MapCameraPosition
-  userLocation(followsHeading:fallback:) 

Type Method

# userLocation(followsHeading:fallback:)

Creates a camera position with the specific fallback position and optionally follows the user’s heading.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
static func userLocation(
    followsHeading: Bool = false,
    fallback: MapCameraPosition
) -> MapCameraPosition
```

## Parameters 

`followsHeading`  

A Boolean value that indicates whether the camera follows the person’s heading.

`fallback`  

A fallback position to use if the map hasn’t resolved the person’s location.

## Return Value

A new MapCameraPosition.

## See Also

### Creating a camera position

static func camera(MapCamera) -> MapCameraPosition

Creates a new camera position from an existing map camera you provide.

static func item(MKMapItem, allowsAutomaticPitch: Bool) -> MapCameraPosition

Creates a new camera position centered on a map item and automatic pitch selection you provide.

static func rect(MKMapRect) -> MapCameraPosition

Creates a new camera position with the map boundaries you provide.

static func region(MKCoordinateRegion) -> MapCameraPosition

Creates a new camera position the coordinate region you provide.

