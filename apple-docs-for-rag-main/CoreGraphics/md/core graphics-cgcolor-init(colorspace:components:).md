

- Core Graphics
- CGColor
-  init(colorSpace:components:) 

Initializer

# init(colorSpace:components:)

Creates a color using a list of intensity values (including alpha) and an associated color space.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.3+tvOSvisionOS 1.0+watchOS 2.0+

``` source
init?(
    colorSpace space: CGColorSpace,
    components: UnsafePointer
)
```

## Parameters 

`space`  

A color space for the new color. Core Graphics retains this object; upon return, you may safely release it.

`components`  

An array of intensity values describing the color. The array should contain *n*+1 values that correspond to the *n* color components in the specified color space, followed by the alpha component. Each component value should be in the range appropriate for the color space. Values outside this range will be clamped to the nearest correct value.

## Return Value

A new color. In Objective-C, you’re responsible for releasing this object using CGColorRelease.

## See Also

### Creating Colors

func copy() -> CGColor?

Creates a copy of an existing color.

func copy(alpha: CGFloat) -> CGColor?

Creates a copy of an existing color, substituting a new alpha value.

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

init?(patternSpace: CGColorSpace, pattern: CGPattern, components: UnsafePointer&lt;CGFloat>)

Creates a color using a list of intensity values (including alpha), a pattern color space, and a pattern.

