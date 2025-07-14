

- Accelerate
- vImage
- vImage.PixelBuffer
-  unpremultiply(alpha:) 

Instance Method

# unpremultiply(alpha:)

Transforms an 8-bit planar pixel buffer in-place from premultiplied alpha format to nonpremultiplied alpha format.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func unpremultiply(alpha: vImage.PixelBuffer)
```

Available when `Format` is `vImage.Planar8`.

## Parameters 

`alpha`  

An 8-bit planar pixel buffer that contains the alpha.

## Discussion

This function divides the color values in `self` by the corresponding alpha values. The function treats the values `0 ... 255` in both pixel buffers as the values `0 ... 1`. For example, the following code premultiplies a 4 x 1 planar pixel buffer with the corresponding pixels in a separate planar alpha buffer:

```
let src = vImage.PixelBuffer(
    pixelValues: [32, 64, 128, 255],
    size: vImage.Size(width: 4, height: 1))

let alpha = vImage.PixelBuffer(
    pixelValues: [0, 128, 128, 255],
    size: vImage.Size(width: 4, height: 1))

src.unpremultiply(alpha: alpha)

// Prints "[0, 128, 255, 255]".
print(src.array)
```

## See Also

### Unpremultiply

func unpremultiply(alpha: vImage.PixelBuffer&lt;Format>)

Transforms a 32-bit planar pixel buffer in-place from premultiplied alpha format to nonpremultiplied alpha format.

func unpremultiply(channelOrdering: vImage.ChannelOrdering)

Transforms an 8-bit ARGB or RGBA pixel buffer in-place from premultiplied alpha format to nonpremultiplied alpha format.

func unpremultiply(channelOrdering: vImage.ChannelOrdering)

Transforms an unsigned 16-bit ARGB or RGBA pixel buffer in-place from premultiplied alpha format to nonpremultiplied alpha format.

func unpremultiply()

Transforms a floating-point 16-bit RGBA pixel buffer in-place from premultiplied alpha format to nonpremultiplied alpha format.

func unpremultiply(channelOrdering: vImage.ChannelOrdering)

Transforms a 32-bit ARGB or RGBA pixel buffer in-place from premultiplied alpha format to nonpremultiplied alpha format.

