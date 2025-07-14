

- Core Image
- CIColor
-  init(red:green:blue:colorSpace:) 

Initializer

# init(red:green:blue:colorSpace:)

Initializes a Core Image color object with the specified red, green, and blue component values as measured in the specified color space.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
convenience init?(
    red r: CGFloat,
    green g: CGFloat,
    blue b: CGFloat,
    colorSpace: CGColorSpace
)
```

## Parameters 

`r`  

The unpremultiplied red component of the color.

`g`  

The unpremultiplied green component of the color.

`b`  

The unpremultiplied blue component of the color.

`colorSpace`  

The color space in which to create the new color. This color space must conform to the CGColorSpaceModel.rgb color space model.

## Return Value

The resulting Core Image color.

## See Also

### Initializing Color Objects

init(cgColor: CGColor)

Initializes a Core Image color object with a Core Graphics color.

init(color: UIColor)

Initializes a Core Image color object using a UIKit (or AppKit) color object.

init(red: CGFloat, green: CGFloat, blue: CGFloat, alpha: CGFloat)

Initializes a Core Image color object with the specified red, green, blue, and alpha component values.

init?(red: CGFloat, green: CGFloat, blue: CGFloat, alpha: CGFloat, colorSpace: CGColorSpace)

Initializes a Core Image color object with the specified red, green, blue, and alpha component values as measured in the specified color space.

