

- Accelerate
- vImage
- vImage.PixelBuffer
-  flatten(channelOrdering:backgroundColor:isPremultiplied:destination:) 

Instance Method

# flatten(channelOrdering:backgroundColor:isPremultiplied:destination:)

Transforms an 8-bit-per-channel RGBA or ARGB buffer to an RGB buffer against an opaque background color.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func flatten(
    channelOrdering: vImage.ChannelOrdering,
    backgroundColor: Pixel_8888,
    isPremultiplied: Bool,
    destination: vImage.PixelBuffer
)
```

Available when `Format` is `vImage.Interleaved8x4`.

## Parameters 

`channelOrdering`  

The channel ordering of the source buffer.

`backgroundColor`  

The background color that the function composites against.

`isPremultiplied`  

A Boolean values that specifies whether the source image is premultiplied.

`destination`  

The destination pixel buffer.

## See Also

### Flattening Channels

func flatten(channelOrdering: vImage.ChannelOrdering, backgroundColor: Pixel_FFFF, isPremultiplied: Bool, destination: vImage.PixelBuffer&lt;vImage.InterleavedFx3>)

Transforms an 32-bit-per-channel RGBA or ARGB buffer to an RGB buffer against an opaque background color.

enum ChannelOrdering

Constants that specify the channel ordering of a pixel buffer.

