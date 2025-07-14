

- MapKit
- MapCamera
-  init(centerCoordinate:distance:heading:pitch:) 

Initializer

# init(centerCoordinate:distance:heading:pitch:)

Creates a camera using the specified distance, pitch, and heading information.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
init(
    centerCoordinate: CLLocationCoordinate2D,
    distance: Double,
    heading: Double = 0,
    pitch: Double = 0
)
```

## Parameters 

`centerCoordinate`  

The map coordinate at the center of the map view.

`distance`  

The distance from the center point of the map to the camera, in meters.

`heading`  

The heading of the camera, in degrees, relative to true North.

`pitch`  

The viewing angle of the camera, in degrees.

## See Also

### Creating a map camera

init(MKMapCamera)

Creates a map camera from the given MapKit camera object.

