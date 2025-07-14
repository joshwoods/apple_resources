

- Foundation
- NSValue
-  mkCoordinateValue 

Instance Property

# mkCoordinateValue

The CoreLocation geographic coordinate structure representation of the value.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.2+visionOS 1.0+watchOS 2.0+

``` source
var mkCoordinateValue: CLLocationCoordinate2D { get }
```

## See Also

### Related Documentation

struct CLLocationCoordinate2D

The latitude and longitude associated with a location, specified using the WGS 84 reference frame.

### Working with Geographic Coordinate Values

init(MKCoordinate: CLLocationCoordinate2D)

Creates a new value object containing the specified CoreLocation geographic coordinate structure.

init(MKCoordinateSpan: MKCoordinateSpan)

Creates a new value object containing the specified MapKit coordinate span structure.

var mkCoordinateSpanValue: MKCoordinateSpan

The MapKit coordinate span structure representation of the value.

