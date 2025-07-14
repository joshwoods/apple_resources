

- Core Graphics
- CGColor
-  copy(alpha:) 

Instance Method

# copy(alpha:)

Creates a copy of an existing color, substituting a new alpha value.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.3+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func copy(alpha: CGFloat) -> CGColor?
```

## Parameters 

`alpha`  

A value that specifies the desired opacity of the copy. Values outside the range `[0,1]` are clamped to `0` or `1`.

## Return Value

A copy of the specified color, using the specified alpha value. In Objective-C, you’re responsible for releasing this object using CGColorRelease.

## See Also

### Creating Colors

func copy() -> CGColor?

Creates a copy of an existing color.

init(genericCMYKCyan: CGFloat, magenta: CGFloat, yellow: CGFloat, black: CGFloat, alpha: CGFloat)

Creates a color in the Generic CMYK color space.

init(gray: CGFloat, alpha: CGFloat)

Creates a color in the Generic gray color space.

init(genericGrayGamma2_2Gray: CGFloat, alpha: CGFloat)

Creates a color in the Generic gray color space with a gamma ramp of 2.2.

init(red: CGFloat, green: CGFloat, blue: CGFloat, alpha: CGFloat)

Creates a color in the Generic RGB color space.

init(srgbRed: CGFloat, green: CGFloat, blue: CGFloat, alpha: CGFloat)

Creates a color in the sRGB color space.

init?(colorSpace: CGColorSpace, components: UnsafePointer&lt;CGFloat>)

Creates a color using a list of intensity values (including alpha) and an associated color space.

init?(patternSpace: CGColorSpace, pattern: CGPattern, components: UnsafePointer&lt;CGFloat>)

Creates a color using a list of intensity values (including alpha), a pattern color space, and a pattern.

