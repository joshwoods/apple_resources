

- Foundation
-  NSRect 

Type Alias

# NSRect

A rectangle.

Mac Catalyst 13.0+macOS 10.0+

``` source
typealias NSRect = CGRect
```

## Discussion

When building for 64 bit systems, or building 32 bit like 64 bit, `NSRect` is typedef’d to `CGRect`.

## Topics

### Managing Rectangles

func NSContainsRect(NSRect, NSRect) -> Bool

Returns a Boolean value that indicates whether one rectangle completely encloses another.

func NSDivideRect(NSRect, UnsafeMutablePointer&lt;NSRect>, UnsafeMutablePointer&lt;NSRect>, Double, NSRectEdge)

Divides a rectangle into two new rectangles.

func NSEqualRects(NSRect, NSRect) -> Bool

Returns a Boolean value that indicates whether the two rectangles are equal.

func NSIsEmptyRect(NSRect) -> Bool

Returns a Boolean value that indicates whether a given rectangle is empty.

func NSHeight(NSRect) -> Double

Returns the height of a given rectangle.

func NSInsetRect(NSRect, Double, Double) -> NSRect

Insets a rectangle by a specified amount.

func NSIntegralRect(NSRect) -> NSRect

Adjusts the sides of a rectangle to integer values.

func NSIntegralRectWithOptions(NSRect, AlignmentOptions) -> NSRect

Adjusts the sides of a rectangle to integral values using the specified options.

func NSIntersectionRect(NSRect, NSRect) -> NSRect

Calculates the intersection of two rectangles.

func NSIntersectsRect(NSRect, NSRect) -> Bool

Returns a Boolean value that indicates whether two rectangles intersect.

func NSMakeRect(Double, Double, Double, Double) -> NSRect

Creates a new `NSRect` from the specified values.

func NSMaxX(NSRect) -> Double

Returns the largest x coordinate of a given rectangle.

func NSMaxY(NSRect) -> Double

Returns the largest y coordinate of a given rectangle.

func NSMidX(NSRect) -> Double

Returns the x coordinate of a given rectangle’s midpoint.

func NSMidY(NSRect) -> Double

Returns the y coordinate of a given rectangle’s midpoint.

func NSMinX(NSRect) -> Double

Returns the smallest x coordinate of a given rectangle.

func NSMinY(NSRect) -> Double

Returns the smallest y coordinate of a given rectangle.

func NSMouseInRect(NSPoint, NSRect, Bool) -> Bool

Returns a Boolean value that indicates whether the point is in the specified rectangle.

func NSOffsetRect(NSRect, Double, Double) -> NSRect

Offsets the rectangle by the specified amount.

func NSPointInRect(NSPoint, NSRect) -> Bool

Returns a Boolean value that indicates whether a given point is in a given rectangle.

func NSRectFromString(String) -> NSRect

Returns a rectangle from a text-based representation.

func NSStringFromRect(NSRect) -> String

Returns a string representation of a rectangle.

func NSRectFromCGRect(CGRect) -> NSRect

Returns an `NSRect` typecast from a `CGRect`.

func NSRectToCGRect(NSRect) -> CGRect

Returns a `CGRect` typecast from an `NSRect`.

func NSUnionRect(NSRect, NSRect) -> NSRect

Calculates the union of two rectangles.

func NSWidth(NSRect) -> Double

Returns the width of the specified rectangle.

### Zero Constant

let NSZeroRect: NSRect

An `NSRect` structure set to `0` in width and height.

### Related Types

enum NSRectEdge

struct AlignmentOptions

Values representing alignment operations.

typealias NSRectArray

Type indicating a parameter is array of `NSRect` structures.

typealias NSRectPointer

Type indicating a parameter is a pointer to an `NSRect` structure.

## See Also

### Geometry

@frozen struct CGFloat

The basic type for floating-point scalar values in Core Graphics and related frameworks.

typealias NSPoint

A point in a Cartesian coordinate system.

typealias NSSize

A two-dimensional size.

struct AffineTransform

A graphics coordinate transformation.

struct NSEdgeInsets

A description of the distance between the edges of two rectangles.

