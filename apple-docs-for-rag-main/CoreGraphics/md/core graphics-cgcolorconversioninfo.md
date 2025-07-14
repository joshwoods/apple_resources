

- Core Graphics
-  CGColorConversionInfo 

Class

# CGColorConversionInfo

An object that describes how to convert between color spaces for use by other system services.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class CGColorConversionInfo
```

## Overview

A CGColorConversionInfo object specifies a conversion between two or more color spaces, including information about the intent of the conversion. You use color conversion objects to specify the work to be done by an MPSImageConversion filter, which can then perform GPU-accelerated image conversion.

## Topics

### Creating a Color Conversion

init?(src: CGColorSpace, dst: CGColorSpace)

Creates a conversion between two specified color spaces.

init?(optionsSrc: CGColorSpace, dst: CGColorSpace, options: CFDictionary?)

init?(src: CGColorSpace, srcHeadroom: Float, dst: CGColorSpace, dstHeadroom: Float, toneMapping: CGToneMapping, options: CFDictionary?, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?)

enum CGColorConversionInfoTransformType

Constants describing how a color conversion uses color spaces.

### Working with Core Foundation Types

class var typeID: CFTypeID

Returns the Core Foundation type identifier for a color conversion info data type.

### Instance Methods

func convert(width: Int, height: Int, to: UnsafeMutableRawPointer, format: CGColorBufferFormat, from: UnsafeRawPointer, format: CGColorBufferFormat, options: CFDictionary?) -> Bool

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Colors and Fonts

class CGColor

A set of components that define a color, with a color space specifying how to interpret them.

class CGColorSpace

A profile that specifies how to interpret a color value for display.

class CGFont

A set of character glyphs and layout information for drawing text.

