

- Core Graphics
-  CGColor 

Class

# CGColor

A set of components that define a color, with a color space specifying how to interpret them.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class CGColor
```

## Overview

`CGColor` is the fundamental data type used internally by Core Graphics to represent colors. `CGColor` objects, and the functions that operate on them, provide a fast and convenient way of managing and setting colors directly, especially colors that are reused (such as black for text).

A color object contains a set of components (such as red, green, and blue) that uniquely define a color, and a color space that specifies how those components should be interpreted.

Color objects provide a fast and convenient way to manage and set colors, especially colors that are used repeatedly. Drawing operations use color objects for setting fill and stroke colors, managing alpha, and setting color with a pattern.

CGColor is derived from CFTypeRef and inherits the properties that all Core Foundation types have in common.

## Topics

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

init?(colorSpace: CGColorSpace, components: UnsafePointer&lt;CGFloat>)

Creates a color using a list of intensity values (including alpha) and an associated color space.

init?(patternSpace: CGColorSpace, pattern: CGPattern, components: UnsafePointer&lt;CGFloat>)

Creates a color using a list of intensity values (including alpha), a pattern color space, and a pattern.

### Getting System Colors

class var black: CGColor

The black color in the Generic gray color space.

class var white: CGColor

The white color in the Generic gray color space.

class var clear: CGColor

The clear color in the Generic gray color space.

### Examining a Color

var alpha: CGFloat

Returns the value of the alpha component associated with a color.

var colorSpace: CGColorSpace?

Returns the color space associated with a color.

var components: [CGFloat]?

Returns the values of the color components (including alpha) associated with a color.

var numberOfComponents: Int

Returns the number of color components (including alpha) associated with a color.

var pattern: CGPattern?

Returns the pattern associated with a color in a pattern color space.

### Converting Between Color Spaces

class let conversionTRCSize: CFString

func converted(to: CGColorSpace, intent: CGColorRenderingIntent, options: CFDictionary?) -> CGColor?

Creates a new color in a different color space that matches the provided color.

### Working with Core Foundation Types

class var typeID: CFTypeID

Returns the Core Foundation type identifier for a color data type.

### Type Properties

class let conversionBlackPointCompensation: CFString

An option for whether to apply black point compensation when converting between color profiles.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Related Documentation

Quartz 2D Programming Guide

### Colors and Fonts

class CGColorConversionInfo

An object that describes how to convert between color spaces for use by other system services.

class CGColorSpace

A profile that specifies how to interpret a color value for display.

class CGFont

A set of character glyphs and layout information for drawing text.

