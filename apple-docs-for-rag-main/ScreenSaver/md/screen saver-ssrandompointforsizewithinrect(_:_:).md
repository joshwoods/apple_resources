

- Screen Saver
-  SSRandomPointForSizeWithinRect(\_:\_:) 

Function

# SSRandomPointForSizeWithinRect(\_:\_:)

Returns a random point.

macOS 10.0+

``` source
func SSRandomPointForSizeWithinRect(
    _ size: NSSize,
    _ rect: NSRect
) -> NSPoint
```

## Parameters 

`size`  

The horizontal and vertical amounts to subtract from the rectangle’s size.

`rect`  

The rectangle to contain the point.

## Return Value

A random point within `rect`, constrained within `(rect.size - size)` from `rect`’s origin.

## Discussion

The Screen Saver framework automatically seeds the `random()` C function to generate the point.

## See Also

### Utilities

func SSRandomIntBetween(Int32, Int32) -> Int32

Returns a random integer value.

func SSRandomFloatBetween(CGFloat, CGFloat) -> CGFloat

Returns a random float value.

func SSCenteredRectInRect(NSRect, NSRect) -> NSRect

Returns a rectangle.

