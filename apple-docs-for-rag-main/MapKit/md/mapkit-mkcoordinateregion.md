

- MapKit
-  MKCoordinateRegion 

Structure

# MKCoordinateRegion

A rectangular geographic region that centers around a specific latitude and longitude.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct MKCoordinateRegion
```

## Topics

### Creating a region

init()

Creates a coordinate region.

init(center: CLLocationCoordinate2D, latitudinalMeters: CLLocationDistance, longitudinalMeters: CLLocationDistance)

Creates a new coordinate region from the specified coordinate and distance values.

init(MKMapRect)

Returns the region that corresponds to the specified map rectangle.

init(center: CLLocationCoordinate2D, span: MKCoordinateSpan)

Creates a coordinate region with a span around the specified center coordinate.

### Getting the region coordinates

var center: CLLocationCoordinate2D

The center point of the region.

var span: MKCoordinateSpan

The horizontal and vertical span representing the amount of map to display.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Map coordinates

struct MKCoordinateSpan

The width and height of a map region.

struct MKMapRect

A rectangular area on a two-dimensional map projection.

struct MKMapPoint

A point on a two-dimensional map projection.

struct MKMapSize

Width and height information on a two-dimensional map projection.

class MKDistanceFormatter

A utility object that converts between a geographic distance and a string-based expression of that distance.

