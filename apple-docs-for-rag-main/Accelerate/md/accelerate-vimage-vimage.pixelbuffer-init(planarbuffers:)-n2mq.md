

- Accelerate
- vImage
- vImage.PixelBuffer
-  init(planarBuffers:) 

Initializer

# init(planarBuffers:)

Creates a 2-channel, 32-bit-per-channel interleaved buffer from two 32-bit planar buffers.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
init(planarBuffers: [vImage.PixelBuffer])
```

Available when `Format` is `vImage.InterleavedFx2`.

## Parameters 

`planarBuffers`  

An array that contains two 32-bit planar buffers.

## Discussion

Use this function to interleave two discrete planar buffers. For example, the following code creates a two-channel buffer from two planar buffers:

```
let planar0 = vImage.PixelBuffer(
    pixelValues: [Float(0.125), Float(0.5)],
    size: vImage.Size(width: 2, height: 1))

let planar1 = vImage.PixelBuffer(
    pixelValues: [Float(0.25), Float(1)],
    size: vImage.Size(width: 2, height: 1))

let interleaved = vImage.PixelBuffer(
    planarBuffers: [planar0, planar1])

// Prints "[0.125, 0.25, 0.5, 1]"
print(interleaved.array)
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

Creates a 3-channel, 32-bit-per-channel interleaved buffer from three 32-bit planar buffers.

init(planarBuffers: [vImage.PixelBuffer&lt;vImage.PlanarF>])

Creates a 4-channel, 32-bit-per-channel interleaved buffer from four 32-bit planar buffers.

init(planarBuffers: [vImage.PixelBuffer&lt;vImage.Planar16U>])

Creates a 4-channel, 16-bit-per-channel interleaved buffer from four 16-bit planar buffers.

init(lumaSource: vImage.PixelBuffer&lt;vImage.Planar8>, chromaSource: vImage.PixelBuffer&lt;vImage.Interleaved8x2>, conversionInfo: vImage_YpCbCrToARGB)

Creates a 4-channel, 8-bit-per-channel interleaved buffer from a planar Yp buffer and a two-channel interleaved CbCr buffer.

init(interleavedBuffer: vImage.PixelBuffer&lt;vImage.Interleaved8x4>)

Creates a 4-channel, 32-bit-per-channel interleaved buffer from a 4-channel, 8-bit-per-channel interleaved buffer.

