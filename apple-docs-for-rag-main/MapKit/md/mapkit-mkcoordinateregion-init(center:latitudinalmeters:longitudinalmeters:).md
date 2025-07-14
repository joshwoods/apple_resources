

- MapKit
- MKCoordinateRegion
-  init(center:latitudinalMeters:longitudinalMeters:) 

Initializer

# init(center:latitudinalMeters:longitudinalMeters:)

Creates a new coordinate region from the specified coordinate and distance values.

iOSiPadOSMac CatalystmacOStvOS 9.2+visionOSwatchOS

``` source
init(
    center centerCoordinate: CLLocationCoordinate2D,
    latitudinalMeters: CLLocationDistance,
    longitudinalMeters: CLLocationDistance
)
```

## Parameters 

`centerCoordinate`  

The center point of the new coordinate region.

`latitudinalMeters`  

The north-to-south span of the region (measured in meters) specified as the distance from the center point to the bounds along the north-to-south axis.

`longitudinalMeters`  

The east-to-west span of the region (measured in meters) specified as the distance from the center point to the bounds along the east-to-west axis.

## Return Value

A region with the specified values.

## See Also

### Creating a region

init()

Creates a coordinate region.

init(MKMapRect)

Returns the region that corresponds to the specified map rectangle.

init(center: CLLocationCoordinate2D, span: MKCoordinateSpan)

Creates a coordinate region with a span around the specified center coordinate.

