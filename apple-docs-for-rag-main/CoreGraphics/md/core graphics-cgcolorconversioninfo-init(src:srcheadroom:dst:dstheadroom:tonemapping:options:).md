

- Core Graphics
- CGColorConversionInfo
-  init(src:srcHeadroom:dst:dstHeadroom:toneMapping:options:) 

Initializer

# init(src:srcHeadroom:dst:dstHeadroom:toneMapping:options:)

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
init?(
    src from: CGColorSpace,
    srcHeadroom source_headroom: Float,
    dst to: CGColorSpace,
    dstHeadroom target_headroom: Float,
    toneMapping method: CGToneMapping,
    options: CFDictionary?,
    _ error: UnsafeMutablePointer?>?
)
```

## See Also

### Creating a Color Conversion

init?(src: CGColorSpace, dst: CGColorSpace)

Creates a conversion between two specified color spaces.

init?(optionsSrc: CGColorSpace, dst: CGColorSpace, options: CFDictionary?)

enum CGColorConversionInfoTransformType

Constants describing how a color conversion uses color spaces.

