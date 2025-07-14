

- Foundation
- NSValue
-  init(MKCoordinate:) 

Initializer

# init(MKCoordinate:)

Creates a new value object containing the specified CoreLocation geographic coordinate structure.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.2+visionOS 1.0+watchOS 2.0+

``` source
init(MKCoordinate coordinate: CLLocationCoordinate2D)
```

``` source
init(mkCoordinate coordinate: CLLocationCoordinate2D)
```

## Parameters 

`coordinate`  

The value for the new object.

## Return Value

A new value object that contains the geographic coordinate information.

## See Also

### Related Documentation

struct CLLocationCoordinate2D

The latitude and longitude associated with a location, specified using the WGS 84 reference frame.

### Working with Geographic Coordinate Values

init(MKCoordinateSpan: MKCoordinateSpan)

Creates a new value object containing the specified MapKit coordinate span structure.

var mkCoordinateValue: CLLocationCoordinate2D

The CoreLocation geographic coordinate structure representation of the value.

var mkCoordinateSpanValue: MKCoordinateSpan

The MapKit coordinate span structure representation of the value.

