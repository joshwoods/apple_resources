

- MapKit
-  MapCameraUpdateContext 

Structure

# MapCameraUpdateContext

A structure that defines additional information about the map camera.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
struct MapCameraUpdateContext
```

## Topics

### Accessing information about the camera

let camera: MapCamera

The current map camera.

let rect: MKMapRect

A map rectangle that approximates the view of the map’s camera.

let region: MKCoordinateRegion

A map region that approximates the view of the map’s camera.

## See Also

### Map customization

struct MapCamera

Defines a virtual viewpoint above the map surface.

struct MapCameraBounds

Defines an optional boundary of an area within which the map’s center needs to remain.

struct MapCameraPosition

A structure that describes how to position the map’s camera within the map.

struct MapCameraUpdateFrequency

A structure that describes when the map camera updates.

