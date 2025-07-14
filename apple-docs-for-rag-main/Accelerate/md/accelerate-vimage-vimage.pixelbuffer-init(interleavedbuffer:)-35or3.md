

- Accelerate
- vImage
- vImage.PixelBuffer
-  init(interleavedBuffer:) 

Initializer

# init(interleavedBuffer:)

Creates a 4-channel, 32-bit-per-channel interleaved buffer from a 4-channel, 8-bit-per-channel interleaved buffer.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
init(interleavedBuffer: vImage.PixelBuffer)
```

Available when `Format` is `vImage.InterleavedFx4`.

## Parameters 

`interleavedBuffer`  

The source pixel buffer.

## Discussion

This function treats floating point pixels represented by the range `0 ... 1` as the UInt8 range `0 ... 255`.

For example, the following code initializes an vImage.InterleavedFx4 pixel buffer from a vImage.Interleaved8x4 pixel buffer:

```
let src = vImage.PixelBuffer(
    pixelValues: [255 / 17,
                  255 / 15,
                  255 / 5,
                  255 / 3] as [UInt8],
    size: vImage.Size(width: 1,
                      height: 1))

let dest = vImage.PixelBuffer(interleavedBuffer: src)
```

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

init(lumaSource: vImage.PixelBuffer&lt;vImage.Planar8>, chromaSource: vImage.PixelBuffer&lt;vImage.Interleaved8x2>, conversionInfo: vImage_YpCbCrToARGB)

Creates a 4-channel, 8-bit-per-channel interleaved buffer from a planar Yp buffer and a two-channel interleaved CbCr buffer.

