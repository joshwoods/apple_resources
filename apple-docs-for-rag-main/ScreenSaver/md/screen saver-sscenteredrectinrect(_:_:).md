

- Screen Saver
-  SSCenteredRectInRect(\_:\_:) 

Function

# SSCenteredRectInRect(\_:\_:)

Returns a rectangle.

macOS 10.0+

``` source
func SSCenteredRectInRect(
    _ innerRect: NSRect,
    _ outerRect: NSRect
) -> NSRect
```

## Parameters 

`innerRect`  

The rectangle to center.

`outerRect`  

The rectangle to contain `innerRect`.

## Return Value

A rectangle that’s the same size as `innerRect`, but is centered inside `outerRect`.

## See Also

### Utilities

func SSRandomIntBetween(Int32, Int32) -> Int32

Returns a random integer value.

func SSRandomFloatBetween(CGFloat, CGFloat) -> CGFloat

Returns a random float value.

func SSRandomPointForSizeWithinRect(NSSize, NSRect) -> NSPoint

Returns a random point.

