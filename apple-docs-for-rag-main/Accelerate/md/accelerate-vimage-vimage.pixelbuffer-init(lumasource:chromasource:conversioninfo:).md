

- Accelerate
- vImage
- vImage.PixelBuffer
-  init(lumaSource:chromaSource:conversionInfo:) 

Initializer

# init(lumaSource:chromaSource:conversionInfo:)

Creates a 4-channel, 8-bit-per-channel interleaved buffer from a planar Yp buffer and a two-channel interleaved CbCr buffer.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
init(
    lumaSource: vImage.PixelBuffer,
    chromaSource: vImage.PixelBuffer,
    conversionInfo: vImage_YpCbCrToARGB
)
```

Available when `Format` is `vImage.Interleaved8x4`.

## Parameters 

`lumaSource`  

The source buffer that contains the luminance data.

`chromaSource`  

The source buffer that contains the chrominance data.

`conversionInfo`  

An opaque representation of a 3x3 converson matrix for converting Y’CbCr signals to RGB.

## See Also

### Creating an interleaved buffer from another buffer

init(planarBuffers: [vImage.PixelBuffer&lt;vImage.Planar8>])

Creates a 2-channel, 8-bit-per-channel interleaved buffer from two 8-bit planar buffers.

init(planarBuffers: [vImage.PixelBuffer&lt;vImage.Planar8>])

Creates a 3-channel, 8-bit-per-channel interleaved buffer from three 8-bit planar buffers.

init(planarBuffers: [vImage.PixelBuffer&lt;vImage.Planar8>])

Creates a 4-channel, 8-bit-per-channel interleaved buffer from four 8-bit planar buffers.

init(planarBuffers: [vImage.PixelBuffer&lt;vImage.PlanarF>])

Creates a 4-channel, 8-bit-per-channel interleaved buffer from four 32-bit planar buffers.

init(planarBuffers: [vImage.PixelBuffer&lt;vImage.PlanarF>])

Creates a 2-channel, 32-bit-per-channel interleaved buffer from two 32-bit planar buffers.

init(planarBuffers: [vImage.PixelBuffer&lt;vImage.PlanarF>])

Creates a 3-channel, 32-bit-per-channel interleaved buffer from three 32-bit planar buffers.

init(planarBuffers: [vImage.PixelBuffer&lt;vImage.PlanarF>])

Creates a 4-channel, 32-bit-per-channel interleaved buffer from four 32-bit planar buffers.

init(planarBuffers: [vImage.PixelBuffer&lt;vImage.Planar16U>])

Creates a 4-channel, 16-bit-per-channel interleaved buffer from four 16-bit planar buffers.

init(interleavedBuffer: vImage.PixelBuffer&lt;vImage.Interleaved8x4>)

Creates a 4-channel, 32-bit-per-channel interleaved buffer from a 4-channel, 8-bit-per-channel interleaved buffer.

