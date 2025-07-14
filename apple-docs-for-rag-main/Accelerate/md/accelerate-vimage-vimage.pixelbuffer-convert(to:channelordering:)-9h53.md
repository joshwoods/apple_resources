

- Accelerate
- vImage
- vImage.PixelBuffer
-  convert(to:channelOrdering:) 

Instance Method

# convert(to:channelOrdering:)

Converts the 8-bit-per-channel RGBA or ARGB pixel buffer to RGB.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func convert(
    to destination: vImage.PixelBuffer,
    channelOrdering: vImage.ChannelOrdering
)
```

Available when `Format` is `vImage.Interleaved8x4`.

## Parameters 

`destination`  

The destination pixel buffer.

`channelOrdering`  

An enumeration that specifies whether the source is either ARGB or RGBA.

## See Also

### Conversion from four channels to three channels

func convert(to: vImage.PixelBuffer&lt;vImage.InterleavedFx3>, channelOrdering: vImage.ChannelOrdering)

Converts the 32-bit-per-channel RGBA or ARGB pixel buffer to RGB.

