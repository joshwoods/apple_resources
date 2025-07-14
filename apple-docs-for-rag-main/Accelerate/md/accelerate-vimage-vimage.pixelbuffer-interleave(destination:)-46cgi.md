

- Accelerate
- vImage
- vImage.PixelBuffer
-  interleave(destination:) 

Instance Method

# interleave(destination:)

Interleaves the 8-bit-per-channel, three-channel multiple-plane buffer and writes the result to an interleaved pixel buffer.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func interleave(destination: vImage.PixelBuffer)
```

Available when `Format` is `vImage.Planar8x3`.

## Parameters 

`destination`  

The destination pixel buffer.

## Mentioned in 

Optimizing image-processing performance

## Discussion

Use this function to interleave a buffer and overwrite an interleaved buffer with a copy of the source channels.

## See Also

### Interleaving pixel buffers

func interleave(destination: vImage.PixelBuffer&lt;vImage.Interleaved8x4>)

Interleaves the 8-bit-per-channel, four-channel multiple-plane buffer and writes the result to an interleaved pixel buffer.

func interleave(destination: vImage.PixelBuffer&lt;vImage.InterleavedFx3>)

Interleaves the 32-bit-per-channel, three-channel multiple-plane buffer and writes the result to an interleaved pixel buffer.

func interleave(destination: vImage.PixelBuffer&lt;vImage.InterleavedFx4>)

Interleaves the 32-bit-per-channel, four-channel multiple-plane buffer and writes the result to an interleaved pixel buffer.

func interleave(planarSourceBuffers: [vImage.PixelBuffer&lt;vImage.Planar8>])

Interleaves the specified planar source buffers and writes the result to the 8-bit-per-channel, three-channel interleaved buffer.

func interleave(planarSourceBuffers: [vImage.PixelBuffer&lt;vImage.Planar8>])

Interleaves the specified planar source buffers and writes the result to the 8-bit-per-channel, four-channel interleaved buffer.

func interleave(planarSourceBuffers: [vImage.PixelBuffer&lt;vImage.Planar16F>])

Interleaves the specified planar source buffers and writes the result to the 16-bit-per-channel, four-channel interleaved buffer.

func interleave(planarSourceBuffers: [vImage.PixelBuffer&lt;vImage.Planar16U>])

Interleaves the specified planar source buffers and writes the result to the unsigned 16-bit-per-channel, four-channel interleaved buffer.

func interleave(planarSourceBuffers: [vImage.PixelBuffer&lt;vImage.PlanarF>])

Interleaves the specified planar source buffers and writes the result to the 32-bit-per-channel, three-channel interleaved buffer.

func interleave(planarSourceBuffers: [vImage.PixelBuffer&lt;vImage.PlanarF>])

Interleaves the specified planar source buffers and writes the result to the 32-bit-per-channel, four-channel interleaved buffer.

