

- Accelerate
- vImage
- vImage.PixelBuffer
-  deinterleave(destination:) 

Instance Method

# deinterleave(destination:)

Deinterleaves the 8-bit-per-channel, four-channel interleaved buffer and writes the result to a multiple-plane pixel buffer.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func deinterleave(destination: vImage.PixelBuffer)
```

Available when `Format` is `vImage.Interleaved8x4`.

## Parameters 

`destination`  

The destination pixel buffer.

## Discussion

Use this function to deinterleave a buffer and overwrite a multiple-plane pixel buffer with copies of each source channel.

## See Also

### Deinterleaving pixel buffers

func deinterleave(destination: vImage.PixelBuffer&lt;vImage.Planar8x3>)

Deinterleaves the 8-bit-per-channel, three-channel interleaved buffer and writes the result to a multiple-plane pixel buffer.

func deinterleave(destination: vImage.PixelBuffer&lt;vImage.PlanarFx3>)

Deinterleaves the 32-bit-per-channel, three-channel interleaved buffer and writes the result to a multiple-plane pixel buffer.

func deinterleave(destination: vImage.PixelBuffer&lt;vImage.PlanarFx4>)

Deinterleaves the 32-bit-per-channel, four-channel interleaved buffer and writes the result to a multiple-plane pixel buffer.

func deinterleave(planarDestinationBuffers: [vImage.PixelBuffer&lt;vImage.Planar8>])

Deinterleaves the 8-bit-per-channel, three-channel interleaved buffer and writes the result to an array that contains three planar buffers.

func deinterleave(planarDestinationBuffers: [vImage.PixelBuffer&lt;vImage.Planar8>])

Deinterleaves the 8-bit-per-channel, four-channel interleaved buffer and writes the result to an array that contains four planar buffers.

func deinterleave(planarDestinationBuffers: [vImage.PixelBuffer&lt;vImage.Planar16F>])

Deinterleaves the 16-bit-per-channel, four-channel interleaved buffer and writes the result to an array that contains four planar buffers.

func deinterleave(planarDestinationBuffers: [vImage.PixelBuffer&lt;vImage.Planar16U>])

Deinterleaves the unsigned 16-bit-per-channel, four-channel interleaved buffer and writes the result to an array that contains four planar buffers.

func deinterleave(planarDestinationBuffers: [vImage.PixelBuffer&lt;vImage.PlanarF>])

Deinterleaves the 32-bit-per-channel, three-channel interleaved buffer and writes the result to an array that contains three planar buffers.

func deinterleave(planarDestinationBuffers: [vImage.PixelBuffer&lt;vImage.PlanarF>])

Deinterleaves the 32-bit-per-channel, four-channel interleaved buffer and writes the result to an array that contains four planar buffers.

