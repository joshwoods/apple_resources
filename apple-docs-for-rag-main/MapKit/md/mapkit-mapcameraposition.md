

- MapKit
-  MapCameraPosition 

Structure

# MapCameraPosition

A structure that describes how to position the map’s camera within the map.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
struct MapCameraPosition
```

## Overview

`MapCameraPosition` contains a variety of properties that you can use to control the semantic framings of the camera in relation to its position to the map, such as automatic, which frames the content of the map, and the camera property, which allows you to specify an explicit camera position.

When you pass `MapCameraPosition` as a binding to a map, the map adjusts its camera to frame the requested content, or to exactly match the camera `MapCameraPosition` specifies. If a person interacts with the Map in a way that moves the map, the map resets the position to a value that specifies positionedByUser.

## Topics

### Creating a camera position

static func camera(MapCamera) -> MapCameraPosition

Creates a new camera position from an existing map camera you provide.

static func item(MKMapItem, allowsAutomaticPitch: Bool) -> MapCameraPosition

Creates a new camera position centered on a map item and automatic pitch selection you provide.

static func rect(MKMapRect) -> MapCameraPosition

Creates a new camera position with the map boundaries you provide.

static func region(MKCoordinateRegion) -> MapCameraPosition

Creates a new camera position the coordinate region you provide.

static func userLocation(followsHeading: Bool, fallback: MapCameraPosition) -> MapCameraPosition

Creates a camera position with the specific fallback position and optionally follows the user’s heading.

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

var positionedByUser: Bool

A Boolean value that indicates whether the person specified the camera position by interacting with the map.

var rect: MKMapRect?

The position that frames the given map rectangle.

var region: MKCoordinateRegion?

The coordinate region to frame.

### Accessing information about someone’s location

var followsUserHeading: Bool

A Boolean value that indicates whether the map is following someone’s heading.

var followsUserLocation: Bool

A Boolean value that indicates whether the map is following someone’s location.

## Relationships

### Conforms To

- Equatable

## See Also

### Map customization

struct MapCamera

Defines a virtual viewpoint above the map surface.

struct MapCameraBounds

Defines an optional boundary of an area within which the map’s center needs to remain.

struct MapCameraUpdateContext

A structure that defines additional information about the map camera.

struct MapCameraUpdateFrequency

A structure that describes when the map camera updates.

