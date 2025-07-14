

- MapKit
- MKCoordinateRegion
-  init(\_:) 

Initializer

# init(\_:)

Returns the region that corresponds to the specified map rectangle.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+watchOS 2.0+

``` source
init(_ rect: MKMapRect)
```

## Parameters 

`rect`  

The map rectangle that corresponds to the desired region on a two-dimensional map projection.

## Return Value

The region structure specifying the latitude, longitude, and span values for the specified rectangle.

## See Also

### Creating a region

init()

Creates a coordinate region.

init(center: CLLocationCoordinate2D, latitudinalMeters: CLLocationDistance, longitudinalMeters: CLLocationDistance)

Creates a new coordinate region from the specified coordinate and distance values.

init(center: CLLocationCoordinate2D, span: MKCoordinateSpan)

Creates a coordinate region with a span around the specified center coordinate.

