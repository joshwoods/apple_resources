

- Core Image
- CIImageAccumulator
-  init(extent:format:colorSpace:) 

Initializer

# init(extent:format:colorSpace:)

Initializes an image accumulator with the specified extent, pixel format, and color space.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
init?(
    extent: CGRect,
    format: CIFormat,
    colorSpace: CGColorSpace
)
```

## Parameters 

`extent`  

A rectangle that specifies the x-value of the rectangle origin, the y-value of the rectangle origin, and the width and height.

`format`  

The format and size of each pixel. You must supply a pixel format constant, such askCIFormatARGB8 (32 bit-per-pixel, fixed-point pixel format) or kCIFormatRGBAf (128 bit-per-pixel, floating-point pixel format). See CIImage for more information about pixel format constants.

`colorSpace`  

A CGColorSpace object describing the color space for the image accumulator.

## Return Value

The initialized image accumulator object.

## See Also

### Initializing an Image Accumulator

init?(extent: CGRect, format: CIFormat)

Initializes an image accumulator with the specified extent and pixel format.

### Related Documentation

+ imageAccumulatorWithExtent:format:

Creates an image accumulator with the specified extent and pixel format.

