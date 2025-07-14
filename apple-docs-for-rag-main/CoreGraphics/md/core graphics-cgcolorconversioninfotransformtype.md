

- Core Graphics
-  CGColorConversionInfoTransformType 

Enumeration

# CGColorConversionInfoTransformType

Constants describing how a color conversion uses color spaces.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum CGColorConversionInfoTransformType
```

## Topics

### Enumeration Cases

case transformApplySpace

Specifies a color conversion between one color profile and another.

case transformFromSpace

Specifies a color conversion from a device color space to a color profile.

case transformToSpace

Specifies a color conversion from a color profile to a device color space.

### Initializers

init?(rawValue: UInt32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Creating a Color Conversion

init?(src: CGColorSpace, dst: CGColorSpace)

Creates a conversion between two specified color spaces.

init?(optionsSrc: CGColorSpace, dst: CGColorSpace, options: CFDictionary?)

init?(src: CGColorSpace, srcHeadroom: Float, dst: CGColorSpace, dstHeadroom: Float, toneMapping: CGToneMapping, options: CFDictionary?, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?)

