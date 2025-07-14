

- Foundation
-  NSMakeRect(\_:\_:\_:\_:) 

Function

# NSMakeRect(\_:\_:\_:\_:)

Creates a new `NSRect` from the specified values.

Mac Catalyst 13.0+macOS 10.0+

``` source
func NSMakeRect(
    _ x: Double,
    _ y: Double,
    _ w: Double,
    _ h: Double
) -> NSRect
```

## Return Value

An `NSRect` having the specified origin of \[`x`, `y`\] and size of \[`w`, `h`\].

## See Also

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

