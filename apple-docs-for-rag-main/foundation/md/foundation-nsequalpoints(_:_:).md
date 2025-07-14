

- Foundation
-  NSEqualPoints(\_:\_:) 

Function

# NSEqualPoints(\_:\_:)

Returns a Boolean value that indicates whether two points are equal.

Mac Catalyst 13.0+macOS 10.0+

``` source
func NSEqualPoints(
    _ aPoint: NSPoint,
    _ bPoint: NSPoint
) -> Bool
```

## Return Value

true if the two points `aPoint` and `bPoint` are identical, otherwise false.

## See Also

### Managing Points

func NSMakePoint(Double, Double) -> NSPoint

Creates a new `NSPoint` from the specified values.

func NSPointFromString(String) -> NSPoint

Returns a point from a text-based representation.

func NSStringFromPoint(NSPoint) -> String

Returns a string representation of a point.

func NSPointFromCGPoint(CGPoint) -> NSPoint

Returns an `NSPoint` typecast from a `CGPoint`.

func NSPointToCGPoint(NSPoint) -> CGPoint

Returns a `CGPoint` typecast from an `NSPoint`.

