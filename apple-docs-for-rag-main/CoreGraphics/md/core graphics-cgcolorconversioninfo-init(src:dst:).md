

- Core Graphics
- CGColorConversionInfo
-  init(src:dst:) 

Initializer

# init(src:dst:)

Creates a conversion between two specified color spaces.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
init?(
    src: CGColorSpace,
    dst: CGColorSpace
)
```

## Parameters 

`src`  

The source color space from which color values are to be converted.

`dst`  

The destination color space to which colors are to be converted.

## Return Value

A color conversion object, or `nil` if no conversion between the specified color spaces is allowed.

## Discussion

The source and destination color spaces must be calibrated color spaces (that is, not device-specific or indexed color spaces).

You can use a color conversion object to create MPSImageConversion filters that perform GPU-accelerated color space conversion.

## See Also

### Creating a Color Conversion

init?(optionsSrc: CGColorSpace, dst: CGColorSpace, options: CFDictionary?)

init?(src: CGColorSpace, srcHeadroom: Float, dst: CGColorSpace, dstHeadroom: Float, toneMapping: CGToneMapping, options: CFDictionary?, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?)

enum CGColorConversionInfoTransformType

Constants describing how a color conversion uses color spaces.

