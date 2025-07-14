

- Screen Saver
-  SSRandomFloatBetween(\_:\_:) 

Function

# SSRandomFloatBetween(\_:\_:)

Returns a random float value.

macOS 10.0+

``` source
func SSRandomFloatBetween(
    _ a: CGFloat,
    _ b: CGFloat
) -> CGFloat
```

## Parameters 

`a`  

The first floating-point value.

`b`  

The second floating-point value.

## Return Value

A random floating-point value between the values `a` and `b`, inclusive.

## Discussion

The Screen Saver framework automatically seeds the `random()` C function to generate the number.

## See Also

### Utilities

func SSRandomIntBetween(Int32, Int32) -> Int32

Returns a random integer value.

func SSRandomPointForSizeWithinRect(NSSize, NSRect) -> NSPoint

Returns a random point.

func SSCenteredRectInRect(NSRect, NSRect) -> NSRect

Returns a rectangle.

