

- MapKit
-  MapCameraBounds 

Structure

# MapCameraBounds

Defines an optional boundary of an area within which the map’s center needs to remain.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
struct MapCameraBounds
```

## Overview

Using the `MapCameraBounds` initializers you can also define an optional camera zoom range that limits the distances that a person can zoom the map camera to.

## Topics

### Creating a map camera bounds

init(centerCoordinateBounds: MKCoordinateRegion, minimumDistance: Double?, maximumDistance: Double?)

Creates a camera bounds with the specified region boundary and zoom ranges.

init(centerCoordinateBounds: MKMapRect, minimumDistance: Double?, maximumDistance: Double?)

Creates a camera bounds with the specified map rectangle boundary and zoom ranges.

init(minimumDistance: Double?, maximumDistance: Double?)

Creates a camera bounds with the zoom ranges you specify.

## See Also

### Map customization

struct MapCamera

Defines a virtual viewpoint above the map surface.

struct MapCameraPosition

A structure that describes how to position the map’s camera within the map.

struct MapCameraUpdateContext

A structure that defines additional information about the map camera.

struct MapCameraUpdateFrequency

A structure that describes when the map camera updates.

