

- Accelerate
- vImage
- vImage.PixelBuffer
-  init(interleavedBuffer:) 

Initializer

# init(interleavedBuffer:)

Creates a 4-channel, 8-bit-per-channel mutiple-plane buffer from a 4-channel, 8-bit-per-channel interleaved buffer.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
init(interleavedBuffer: vImage.PixelBuffer)
```

Available when `Format` is `vImage.Planar8x4`.

## Parameters 

`interleavedBuffer`  

The source pixel buffer.

## Discussion

Use this function to deinterleave a pixel buffer and store the result as homogeneous planes that are represented by multiple underlying vImage buffers.

For example, the following code creates a new vImage.Planar8x4 pixel buffer from a vImage.Interleaved8x4 pixel buffer:

```
let src = vImage.PixelBuffer(
    pixelValues: [50, 100, 150, 200] as [UInt8],
    size: vImage.Size(width: 1, height: 1))

let dest = vImage.PixelBuffer(interleavedBuffer: src)

// Prints "[50] [100] [150] [200]"
dest.withUnsafePixelBuffers { pixelBuffers in
    for pixelBuffer in pixelBuffers {
        print(pixelBuffer.array)
    }
}
```

## See Also

### Creating a multiple-plane buffer from an interleaved buffer

init(interleavedBuffer: vImage.PixelBuffer&lt;vImage.Interleaved8x3>)

Creates a 3-channel, 8-bit-per-channel multiple-plane buffer from a 3-channel, 8-bit-per-channel interleaved buffer.

init(interleavedBuffer: vImage.PixelBuffer&lt;vImage.InterleavedFx3>)

Creates a 3-channel, 32-bit-per-channel multiple-plane buffer from a 3-channel, 32-bit-per-channel interleaved buffer.

init(interleavedBuffer: vImage.PixelBuffer&lt;vImage.InterleavedFx4>)

Creates a 4-channel, 32-bit-per-channel multiple-plane buffer from a 4-channel, 32-bit-per-channel interleaved buffer.

