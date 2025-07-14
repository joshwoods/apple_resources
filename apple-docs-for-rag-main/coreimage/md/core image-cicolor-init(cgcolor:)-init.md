

- Core Image
- CIColor
-  init(cgColor:) 

Initializer

# init(cgColor:)

Initializes a Core Image color object with a Core Graphics color.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
init(cgColor c: CGColor)
```

## Parameters 

`c`  

A Core Graphics color value.

## Return Value

The resulting Core Image color.

## Discussion

A CGColor object is the fundamental opaque data type used internally by Core Graphics to represent colors. For more information on Core Graphics color and color spaces, see Quartz 2D Programming Guide.

You can pass a CGColor object that represents any color space, including CMYK, but Core Image converts all color spaces to the Core Image working color space before it passes the color space to the filter kernel. The Core Image working color space uses three color components plus alpha.

## See Also

### Initializing Color Objects

init(color: UIColor)

Initializes a Core Image color object using a UIKit (or AppKit) color object.

init(red: CGFloat, green: CGFloat, blue: CGFloat, alpha: CGFloat)

Initializes a Core Image color object with the specified red, green, blue, and alpha component values.

init?(red: CGFloat, green: CGFloat, blue: CGFloat, colorSpace: CGColorSpace)

Initializes a Core Image color object with the specified red, green, and blue component values as measured in the specified color space.

init?(red: CGFloat, green: CGFloat, blue: CGFloat, alpha: CGFloat, colorSpace: CGColorSpace)

Initializes a Core Image color object with the specified red, green, blue, and alpha component values as measured in the specified color space.

### Related Documentation

Color Management Overview

Core Image Programming Guide

