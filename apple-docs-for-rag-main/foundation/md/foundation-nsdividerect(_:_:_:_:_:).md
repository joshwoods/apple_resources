

- Foundation
-  NSDivideRect(\_:\_:\_:\_:\_:) 

Function

# NSDivideRect(\_:\_:\_:\_:\_:)

Divides a rectangle into two new rectangles.

Mac Catalyst 13.0+macOS 10.0+

``` source
func NSDivideRect(
    _ inRect: NSRect,
    _ slice: UnsafeMutablePointer,
    _ rem: UnsafeMutablePointer,
    _ amount: Double,
    _ edge: NSRectEdge
)
```

## Discussion

Creates two rectangles—`slice` and `rem`—from `inRect`, by dividing `inRect` with a line that’s parallel to the side of `inRect` specified by `edge`. The size of `slice` is determined by `amount`, which specifies the distance from `edge`.

`slice` and `rem` must not be `NULL`.

For more information, see NSRectEdge.

## See Also

### Managing Rectangles

func NSContainsRect(NSRect, NSRect) -> Bool

Returns a Boolean value that indicates whether one rectangle completely encloses another.

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

