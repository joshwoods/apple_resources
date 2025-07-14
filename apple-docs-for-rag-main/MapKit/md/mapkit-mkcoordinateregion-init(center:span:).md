

- MapKit
- MKCoordinateRegion
-  init(center:span:) 

Initializer

# init(center:span:)

Creates a coordinate region with a span around the specified center coordinate.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
init(
    center: CLLocationCoordinate2D,
    span: MKCoordinateSpan
)
```

## Parameters 

`center`  

The center of the coordinate region.

`span`  

The span around the center of the coordinate region.

## See Also

### Creating a region

init()

Creates a coordinate region.

init(center: CLLocationCoordinate2D, latitudinalMeters: CLLocationDistance, longitudinalMeters: CLLocationDistance)

Creates a new coordinate region from the specified coordinate and distance values.

init(MKMapRect)

Returns the region that corresponds to the specified map rectangle.

