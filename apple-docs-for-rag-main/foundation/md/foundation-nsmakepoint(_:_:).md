

- Foundation
-  NSMakePoint(\_:\_:) 

Function

# NSMakePoint(\_:\_:)

Creates a new `NSPoint` from the specified values.

Mac Catalyst 13.0+macOS 10.0+

``` source
func NSMakePoint(
    _ x: Double,
    _ y: Double
) -> NSPoint
```

## Return Value

An `NSPoint` having the coordinates `x` and `y`.

## See Also

### Managing Points

func NSEqualPoints(NSPoint, NSPoint) -> Bool

Returns a Boolean value that indicates whether two points are equal.

func NSPointFromString(String) -> NSPoint

Returns a point from a text-based representation.

func NSStringFromPoint(NSPoint) -> String

Returns a string representation of a point.

func NSPointFromCGPoint(CGPoint) -> NSPoint

Returns an `NSPoint` typecast from a `CGPoint`.

func NSPointToCGPoint(NSPoint) -> CGPoint

Returns a `CGPoint` typecast from an `NSPoint`.

