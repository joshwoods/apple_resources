

- Accelerate
- vImage
- vImage.PixelBuffer
-  convert(lumaSource:chromaSource:conversionInfo:) 

Instance Method

# convert(lumaSource:chromaSource:conversionInfo:)

Populates the pixel buffer with ARGB data from the given luminance and chrominance pixel buffers.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func convert(
    lumaSource: vImage.PixelBuffer,
    chromaSource: vImage.PixelBuffer,
    conversionInfo: vImage_YpCbCrToARGB
)
```

Available when `Format` is `vImage.Interleaved8x4`.

## Parameters 

`lumaSource`  

The source luminance buffer.

`chromaSource`  

The source CbCr chrominance buffer.

`conversionInfo`  

An opaque representation of a 3 x 3 converson matrix for converting Y’CbCr signals to RGB.

