

- SwiftUI
- Color
-  Color.Resolved 

Structure

# Color.Resolved

A concrete color value.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@frozen
struct Resolved
```

## Overview

`Color.Resolved` is a set of RGBA values that represent a color that can be shown. The values are in Linear sRGB color space, extended range. This is a low-level type, most colors are represented by the `Color` type.

See Also

`Color`

## Topics

### Initializers

init(colorSpace: Color.RGBColorSpace, red: Float, green: Float, blue: Float, opacity: Float)

Creates a resolved color from red, green, and blue component values.

### Instance Properties

var blue: Float

The amount of blue in the color in the sRGB color space.

var cgColor: CGColor

A Core Graphics representation of the color.

var green: Float

The amount of green in the color in the sRGB color space.

var linearBlue: Float

The amount of blue in the color in the sRGB linear color space.

var linearGreen: Float

The amount of green in the color in the sRGB linear color space.

var linearRed: Float

The amount of red in the color in the sRGB linear color space.

var opacity: Float

The degree of opacity in the color, given in the range `0` to `1`.

var red: Float

The amount of red in the color in the sRGB color space.

## Relationships

### Conforms To

- Animatable
- BitwiseCopyable
- Copyable
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable
- ShapeStyle

