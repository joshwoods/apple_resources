

- MapKit
-  MapCameraUpdateFrequency 

Structure

# MapCameraUpdateFrequency

A structure that describes when the map camera updates.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
struct MapCameraUpdateFrequency
```

## Topics

### Timing of camera updates

static var continuous: MapCameraUpdateFrequency

A value that indicates that all camera updates are continuous, including while interactions are taking place.

static var onEnd: MapCameraUpdateFrequency

A value that indicates the camera updates when map interactions are complete.

## See Also

### Map customization

struct MapCamera

Defines a virtual viewpoint above the map surface.

struct MapCameraBounds

Defines an optional boundary of an area within which the map’s center needs to remain.

struct MapCameraPosition

A structure that describes how to position the map’s camera within the map.

struct MapCameraUpdateContext

A structure that defines additional information about the map camera.

