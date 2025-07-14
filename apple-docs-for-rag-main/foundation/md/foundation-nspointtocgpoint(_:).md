

- Foundation
-  NSPointToCGPoint(\_:) 

Function

# NSPointToCGPoint(\_:)

Returns a `CGPoint` typecast from an `NSPoint`.

Mac Catalyst 13.0+macOS 10.0+

``` source
func NSPointToCGPoint(_ nspoint: NSPoint) -> CGPoint
```

## Return Value

A `CGPoint` typecast from an `NSPoint`.

## See Also

### Related Documentation

func NSRectToCGRect(NSRect) -> CGRect

Returns a `CGRect` typecast from an `NSRect`.

func NSSizeToCGSize(NSSize) -> CGSize

Returns a `CGSize` typecast from an `NSSize`.

### Managing Points

func NSEqualPoints(NSPoint, NSPoint) -> Bool

Returns a Boolean value that indicates whether two points are equal.

func NSMakePoint(Double, Double) -> NSPoint

Creates a new `NSPoint` from the specified values.

func NSPointFromString(String) -> NSPoint

Returns a point from a text-based representation.

func NSStringFromPoint(NSPoint) -> String

Returns a string representation of a point.

func NSPointFromCGPoint(CGPoint) -> NSPoint

Returns an `NSPoint` typecast from a `CGPoint`.

