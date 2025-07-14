

- MapKit
- MapCircle
-  init(center:radius:) 

Initializer

# init(center:radius:)

Creates a circle with the center coordinate and radius you specify.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
init(
    center coordinate: CLLocationCoordinate2D,
    radius: CLLocationDistance
)
```

## Parameters 

`coordinate`  

The location of the center of the circle.

`radius`  

The radius of the circle, in meters.

## See Also

### Creating a map circle

init(MKCircle)

Creates a circle overlay from an existing map circle object.

init(mapRect: MKMapRect)

Creates the largest possible circle centered within the given map rectangle.

