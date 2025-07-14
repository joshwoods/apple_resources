

- Accelerate
- vImage
- vImage.PixelBuffer
-  permuteChannels(to:destination:) 

Instance Method

# permuteChannels(to:destination:)

Permutes the channels of an 8-bit-per-channel, 4-channel interleaved pixel buffer.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func permuteChannels(
    to permuteMap: (UInt8, UInt8, UInt8, UInt8),
    destination: vImage.PixelBuffer
)
```

Available when `Format` is `vImage.Interleaved8x4`.

## Parameters 

`permuteMap`  

A tuple of four 8-bit integers with the values 0, 1, 2, and 3, in some order.

`destination`  

The destination pixel buffer.

## Discussion

For example, the following code reverses the channel ordering of a pixel buffer:

```
let buffer = vImage.PixelBuffer(
    pixelValues: [10, 20, 30, 40],
    size: vImage.Size(width: 1,
                      height: 1))

buffer.permuteChannels(to: (3, 2, 1, 0),
                       destination: buffer)

// Prints "[40, 30, 20, 10]"
print(buffer.array)
```

## See Also

### Permuting Channels

func permuteChannels(to: (UInt8, UInt8, UInt8), destination: vImage.PixelBuffer&lt;Format>)

Permutes the channels of an 8-bit-per-channel, 3-channel interleaved pixel buffer.

func permuteChannels(to: (UInt8, UInt8, UInt8, UInt8), destination: vImage.PixelBuffer&lt;Format>)

Permutes the channels of an unsigned 16-bit-per-channel, 4-channel interleaved pixel buffer.

func permuteChannels(to: (UInt8, UInt8, UInt8, UInt8), destination: vImage.PixelBuffer&lt;Format>)

Permutes the channels of a floating-point 16-bit-per-channel, 4-channel interleaved pixel buffer.

func permuteChannels(to: (UInt8, UInt8, UInt8, UInt8), destination: vImage.PixelBuffer&lt;Format>)

Permutes the channels of an 32-bit-per-channel, 4-channel interleaved pixel buffer.

