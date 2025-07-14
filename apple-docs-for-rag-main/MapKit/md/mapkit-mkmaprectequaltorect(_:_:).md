

- MapKit
-  MKMapRectEqualToRect(\_:\_:) 

Function

# MKMapRectEqualToRect(\_:\_:)

Returns a Boolean value that indicates whether two map rectangles are equal.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func MKMapRectEqualToRect(
    _ rect1: MKMapRect,
    _ rect2: MKMapRect
) -> Bool
```

## Parameters 

`rect1`  

The first map rectangle.

`rect2`  

The second map rectangle.

## Return Value

true if the rectangles are exactly the same, or false if the origin point or size values are different.

## See Also

### Comparing rectangles

var isNull: Bool

A Boolean value that indicates whether the specified rectangle is null.

var isEmpty: Bool

A Boolean value that indicates whether the specified rectangle has no area.

var spans180thMeridian: Bool

A Boolean value that indicates whether the specified map rectangle crosses the 180th meridian.

var remainder: MKMapRect

A rectangle that represents the normalized portion of the specified rectangle that lies outside the world map boundaries.

