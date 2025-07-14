

- MapKit
- MapCameraPosition
-  item(\_:allowsAutomaticPitch:) 

Type Method

# item(\_:allowsAutomaticPitch:)

Creates a new camera position centered on a map item and automatic pitch selection you provide.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
static func item(
    _ item: MKMapItem,
    allowsAutomaticPitch: Bool = true
) -> MapCameraPosition
```

## Parameters 

`item`  

The MKMapItem to center the map on.

`allowsAutomaticPitch`  

A Boolean value that indicates whether the camera selects a pitch automatically.

## Return Value

Returns a new MapCameraPosition.

## See Also

### Creating a camera position

static func camera(MapCamera) -> MapCameraPosition

Creates a new camera position from an existing map camera you provide.

static func rect(MKMapRect) -> MapCameraPosition

Creates a new camera position with the map boundaries you provide.

static func region(MKCoordinateRegion) -> MapCameraPosition

Creates a new camera position the coordinate region you provide.

static func userLocation(followsHeading: Bool, fallback: MapCameraPosition) -> MapCameraPosition

Creates a camera position with the specific fallback position and optionally follows the user’s heading.

