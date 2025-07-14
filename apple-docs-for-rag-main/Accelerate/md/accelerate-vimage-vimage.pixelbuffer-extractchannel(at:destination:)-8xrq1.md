

- Accelerate
- vImage
- vImage.PixelBuffer
-  extractChannel(at:destination:) 

Instance Method

# extractChannel(at:destination:)

Extracts a single channel from an 32-bit-per-channel, 4-channel interleaved pixel buffer.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func extractChannel(
    at channelIndex: Int,
    destination: vImage.PixelBuffer
)
```

Available when `Format` is `vImage.InterleavedFx4`.

## Parameters 

`channelIndex`  

The index of the channel that the function extracts.

`destination`  

The destination pixel buffer.

## Discussion

For example, the following code extracts channel \`2\` from a four-channel pixel buffer.

```
let src = vImage.PixelBuffer(
    pixelValues: [0.10, 0.11, 0.12, 0.13,
                  0.20, 0.21, 0.22, 0.23,
                  0.30, 0.31, 0.32, 0.33],
    size: vImage.Size(width: 1, height: 3))

let dest = vImage.PixelBuffer(
    size: src.size)

src.extractChannel(at: 2,
                   destination: dest)

// Prints "[0.12, 0.22, 0.32]"
print(dest.array)
```

## See Also

### Extracting Channels

func extractChannel(at: Int, destination: vImage.PixelBuffer&lt;vImage.Planar8>)

Extracts a single channel from an 8-bit-per-channel, 4-channel interleaved pixel buffer.

func extractChannel(at: Int, destination: vImage.PixelBuffer&lt;vImage.Planar16U>)

Extracts a single channel from an unsigned 16-bit-per-channel, 4-channel interleaved pixel buffer.

