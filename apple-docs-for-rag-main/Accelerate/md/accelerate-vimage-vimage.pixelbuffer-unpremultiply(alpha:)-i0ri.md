

- Accelerate
- vImage
- vImage.PixelBuffer
-  unpremultiply(alpha:) 

Instance Method

# unpremultiply(alpha:)

Transforms a 32-bit planar pixel buffer in-place from premultiplied alpha format to nonpremultiplied alpha format.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func unpremultiply(alpha: vImage.PixelBuffer)
```

Available when `Format` is `vImage.PlanarF`.

## Parameters 

`alpha`  

An 32-bit planar pixel buffer that contains the alpha.

## Discussion

This function divides the color values in `self` by the corresponding alpha values. For example, the following code premultiplies a 4 x 1 planar pixel buffer with the corresponding pixels in a separate planar alpha buffer:

```
let src = vImage.PixelBuffer(
    pixelValues: [0.125, 0.25, 0.5, 1],
    size: vImage.Size(width: 4, height: 1))

let alpha = vImage.PixelBuffer(
    pixelValues: [0, 0.25, 0.5, 1],
    size: vImage.Size(width: 4, height: 1))

src.unpremultiply(alpha: alpha)

// Prints "[0.0, ~1.0, ~1.0, ~1.0]".
print(src.array)

```

## See Also

### Unpremultiply

func unpremultiply(alpha: vImage.PixelBuffer&lt;Format>)

Transforms an 8-bit planar pixel buffer in-place from premultiplied alpha format to nonpremultiplied alpha format.

func unpremultiply(channelOrdering: vImage.ChannelOrdering)

Transforms an 8-bit ARGB or RGBA pixel buffer in-place from premultiplied alpha format to nonpremultiplied alpha format.

func unpremultiply(channelOrdering: vImage.ChannelOrdering)

Transforms an unsigned 16-bit ARGB or RGBA pixel buffer in-place from premultiplied alpha format to nonpremultiplied alpha format.

func unpremultiply()

Transforms a floating-point 16-bit RGBA pixel buffer in-place from premultiplied alpha format to nonpremultiplied alpha format.

func unpremultiply(channelOrdering: vImage.ChannelOrdering)

Transforms a 32-bit ARGB or RGBA pixel buffer in-place from premultiplied alpha format to nonpremultiplied alpha format.

