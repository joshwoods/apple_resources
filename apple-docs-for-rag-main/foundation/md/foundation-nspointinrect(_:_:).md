

- Foundation
-  NSPointInRect(\_:\_:) 

Function

# NSPointInRect(\_:\_:)

Returns a Boolean value that indicates whether a given point is in a given rectangle.

Mac Catalyst 13.0+macOS 10.0+

``` source
func NSPointInRect(
    _ aPoint: NSPoint,
    _ aRect: NSRect
) -> Bool
```

## Return Value

true if `aPoint` is located within the rectangle represented by `aRect`, otherwise false.

## Discussion

Point-in-rectangle functions generally assume that the “upper” and “left” edges of a rectangle are inside the rectangle boundaries, while the “lower” and “right” edges are outside the boundaries. This method treats the “upper” and “left” edges of the rectangle as the ones containing the origin of the rectangle.

### Special Considerations

The meanings of “upper” and “lower” (and “left” and “right”) are relative to the current coordinate system and the location of the rectangle. For a rectangle of positive height located in positive x and y coordinates:

- In the default macOS desktop coordinate system—where the origin is at the bottom left—the rectangle edge closest to the bottom of the screen is the “upper” edge (and is considered inside the rectangle).

- On iOS and in a flipped coordinate system in macOS desktop—where the origin is at the top left—the rectangle edge closest to the bottom of the screen is the “lower” edge (and is considered outside the rectangle).

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

