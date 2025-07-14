

- Screen Saver
-  SSRandomIntBetween(\_:\_:) 

Function

# SSRandomIntBetween(\_:\_:)

Returns a random integer value.

macOS 10.0+

``` source
func SSRandomIntBetween(
    _ a: Int32,
    _ b: Int32
) -> Int32
```

## Parameters 

`a`  

The first integer value.

`b`  

The second integer value.

## Discussion

The Screen Saver framework automatically seeds the `random()` C function to generate the number.

## See Also

### Utilities

func SSRandomFloatBetween(CGFloat, CGFloat) -> CGFloat

Returns a random float value.

func SSRandomPointForSizeWithinRect(NSSize, NSRect) -> NSPoint

Returns a random point.

func SSCenteredRectInRect(NSRect, NSRect) -> NSRect

Returns a rectangle.

