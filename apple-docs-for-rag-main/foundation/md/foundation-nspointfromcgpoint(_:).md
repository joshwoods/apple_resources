

- Foundation
-  NSPointFromCGPoint(\_:) 

Function

# NSPointFromCGPoint(\_:)

Returns an `NSPoint` typecast from a `CGPoint`.

Mac Catalyst 13.0+macOS 10.0+

``` source
func NSPointFromCGPoint(_ cgpoint: CGPoint) -> NSPoint
```

## Return Value

An `NSPoint` typecast from a `CGPoint`.

## See Also

### Related Documentation

func NSRectFromCGRect(CGRect) -> NSRect

Returns an `NSRect` typecast from a `CGRect`.

func NSSizeFromCGSize(CGSize) -> NSSize

Returns an `NSSize` typecast from a `CGSize`.

### Managing Points

func NSEqualPoints(NSPoint, NSPoint) -> Bool

Returns a Boolean value that indicates whether two points are equal.

func NSMakePoint(Double, Double) -> NSPoint

Creates a new `NSPoint` from the specified values.

func NSPointFromString(String) -> NSPoint

Returns a point from a text-based representation.

func NSStringFromPoint(NSPoint) -> String

Returns a string representation of a point.

func NSPointToCGPoint(NSPoint) -> CGPoint

Returns a `CGPoint` typecast from an `NSPoint`.

