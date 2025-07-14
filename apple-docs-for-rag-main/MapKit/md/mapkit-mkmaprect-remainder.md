

- MapKit
- MKMapRect
-  remainder 

Instance Property

# remainder

A rectangle that represents the normalized portion of the specified rectangle that lies outside the world map boundaries.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+watchOS 2.0+

``` source
var remainder: MKMapRect { get }
```

## Discussion

For a rectangle that lies on the 180th meridian, this function isolates the portion that lies outside the boundary, wraps it to the opposite side of the map, and returns that rectangle.

## See Also

### Comparing rectangles

var isNull: Bool

A Boolean value that indicates whether the specified rectangle is null.

func MKMapRectEqualToRect(MKMapRect, MKMapRect) -> Bool

Returns a Boolean value that indicates whether two map rectangles are equal.

var isEmpty: Bool

A Boolean value that indicates whether the specified rectangle has no area.

var spans180thMeridian: Bool

A Boolean value that indicates whether the specified map rectangle crosses the 180th meridian.

