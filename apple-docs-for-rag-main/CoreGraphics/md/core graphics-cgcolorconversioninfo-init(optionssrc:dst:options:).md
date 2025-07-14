

- Core Graphics
- CGColorConversionInfo
-  init(optionsSrc:dst:options:) 

Initializer

# init(optionsSrc:dst:options:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.14.6+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init?(
    optionsSrc src: CGColorSpace,
    dst: CGColorSpace,
    options: CFDictionary?
)
```

## See Also

### Creating a Color Conversion

init?(src: CGColorSpace, dst: CGColorSpace)

Creates a conversion between two specified color spaces.

init?(src: CGColorSpace, srcHeadroom: Float, dst: CGColorSpace, dstHeadroom: Float, toneMapping: CGToneMapping, options: CFDictionary?, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?)

enum CGColorConversionInfoTransformType

Constants describing how a color conversion uses color spaces.

