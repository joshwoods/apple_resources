

- MapKit
- MKMapRect
-  isNull 

Instance Property

# isNull

A Boolean value that indicates whether the specified rectangle is null.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var isNull: Bool { get }
```

## Discussion

For this class, a rectangle is `null` if its origin point contains an invalid or infinite value.

## See Also

### Comparing rectangles

func MKMapRectEqualToRect(MKMapRect, MKMapRect) -> Bool

Returns a Boolean value that indicates whether two map rectangles are equal.

var isEmpty: Bool

A Boolean value that indicates whether the specified rectangle has no area.

var spans180thMeridian: Bool

A Boolean value that indicates whether the specified map rectangle crosses the 180th meridian.

var remainder: MKMapRect

A rectangle that represents the normalized portion of the specified rectangle that lies outside the world map boundaries.

