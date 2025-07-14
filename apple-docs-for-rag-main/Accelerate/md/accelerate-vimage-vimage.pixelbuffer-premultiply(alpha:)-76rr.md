

- Accelerate
- vImage
- vImage.PixelBuffer
-  premultiply(alpha:) 

Instance Method

# premultiply(alpha:)

Transforms a 32-bit planar pixel buffer in-place from nonpremultiplied alpha format to premultiplied alpha format.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func premultiply(alpha: vImage.PixelBuffer)
```

Available when `Format` is `vImage.PlanarF`.

## Parameters 

`alpha`  

An 32-bit planar pixel buffer that contains the alpha.

## Discussion

This function multiplies the color values in `self` by the corresponding alpha values. For example, the following code premultiplies a 4 x 1 planar pixel buffer with the corresponding pixels in a separate planar alpha buffer:

```
let src = vImage.PixelBuffer(
    pixelValues: [0.125, 0.25, 0.5, 1],
    size: vImage.Size(width: 4, height: 1))

let alpha = vImage.PixelBuffer(
    pixelValues: [0, 0.25, 0.5, 1],
    size: vImage.Size(width: 4, height: 1))

src.premultiply(alpha: alpha)

// Prints "[0, 0.0625, 0.25, 1]".
print(src.array)

```

## See Also

### Premultiply

func premultiply(alpha: vImage.PixelBuffer&lt;Format>)

Transforms an 8-bit planar pixel buffer in-place from nonpremultiplied alpha format to premultiplied alpha format.

func premultiply(channelOrdering: vImage.ChannelOrdering)

Transforms an 8-bit ARGB or RGBA pixel buffer in-place from nonpremultiplied alpha format to premultiplied alpha format.

func premultiply(channelOrdering: vImage.ChannelOrdering)

Transforms an unsigned 16-bit ARGB or RGBA pixel buffer in-place from nonpremultiplied alpha format to premultiplied alpha format.

func premultiply()

Transforms a floating-point 16-bit RGBA pixel buffer in-place from nonpremultiplied alpha format to premultiplied alpha format.

func premultiply(channelOrdering: vImage.ChannelOrdering)

Transforms a floating-point 32-bit ARGB or RGBA pixel buffer in-place from nonpremultiplied alpha format to premultiplied alpha format.

