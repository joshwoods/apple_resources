

- Foundation
-  NSPoint 

Type Alias

# NSPoint

A point in a Cartesian coordinate system.

Mac Catalyst 13.0+macOS 10.0+

``` source
typealias NSPoint = CGPoint
```

## Discussion

Prior to OS X v10.5 the coordinates were represented by `float` values rather than `CGFloat` values.

When building for 64 bit systems, or building 32 bit like 64 bit, `NSPoint` is typedef’d to `CGPoint`.

## Topics

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

func NSPointToCGPoint(NSPoint) -> CGPoint

Returns a `CGPoint` typecast from an `NSPoint`.

### Zero Constant

let NSZeroPoint: NSPoint

An `NSPoint` structure with both x and y coordinates set to `0`.

### Related Types

typealias NSPointArray

Type indicating a parameter is array of `NSPoint` structures.

typealias NSPointPointer

Type indicating a parameter is a pointer to an `NSPoint` structure.

## See Also

### Geometry

@frozen struct CGFloat

The basic type for floating-point scalar values in Core Graphics and related frameworks.

typealias NSSize

A two-dimensional size.

typealias NSRect

A rectangle.

struct AffineTransform

A graphics coordinate transformation.

struct NSEdgeInsets

A description of the distance between the edges of two rectangles.

