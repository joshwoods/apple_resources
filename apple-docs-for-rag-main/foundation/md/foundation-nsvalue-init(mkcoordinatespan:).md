

- Foundation
- NSValue
-  init(MKCoordinateSpan:) 

Initializer

# init(MKCoordinateSpan:)

Creates a new value object containing the specified MapKit coordinate span structure.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.2+visionOS 1.0+watchOS 2.0+

``` source
init(MKCoordinateSpan span: MKCoordinateSpan)
```

``` source
init(mkCoordinateSpan span: MKCoordinateSpan)
```

## Parameters 

`span`  

The value for the new object.

## Return Value

A new value object that contains the coordinate span information.

## See Also

### Related Documentation

struct MKCoordinateSpan

The width and height of a map region.

### Working with Geographic Coordinate Values

init(MKCoordinate: CLLocationCoordinate2D)

Creates a new value object containing the specified CoreLocation geographic coordinate structure.

var mkCoordinateValue: CLLocationCoordinate2D

The CoreLocation geographic coordinate structure representation of the value.

var mkCoordinateSpanValue: MKCoordinateSpan

The MapKit coordinate span structure representation of the value.

