

- MapKit
-  MapCamera 

Structure

# MapCamera

Defines a virtual viewpoint above the map surface.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
struct MapCamera
```

## Overview

`MapCamera` allows you to specify the viewpoint of a Map, as well as affect how MapKit presents the map to the user.

To create a map view with a 3D perspective, `MapCamera` takes input from the camera and device:

- The location of the camera on the map.

- The compass heading to indicate the camera’s viewing direction.

- The pitch of the camera relative to the map perpendicular.

- The camera’s distance from the target point.

## Topics

### Creating a map camera

init(MKMapCamera)

Creates a map camera from the given MapKit camera object.

init(centerCoordinate: CLLocationCoordinate2D, distance: Double, heading: Double, pitch: Double)

Creates a camera using the specified distance, pitch, and heading information.

### Accessing the camera properties

var centerCoordinate: CLLocationCoordinate2D

The map coordinate at the center of the map view.

var distance: Double

The distance from the center point of the map to the camera, in meters.

var heading: Double

The heading of the camera, in degrees, relative to true North.

var pitch: Double

The viewing angle of the camera, in degrees.

## Relationships

### Conforms To

- Equatable

## See Also

### Map customization

struct MapCameraBounds

Defines an optional boundary of an area within which the map’s center needs to remain.

struct MapCameraPosition

A structure that describes how to position the map’s camera within the map.

struct MapCameraUpdateContext

A structure that defines additional information about the map camera.

struct MapCameraUpdateFrequency

A structure that describes when the map camera updates.

