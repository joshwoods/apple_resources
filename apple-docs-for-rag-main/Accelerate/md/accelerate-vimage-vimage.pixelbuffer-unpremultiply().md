

- Accelerate
- vImage
- vImage.PixelBuffer
-  unpremultiply() 

Instance Method

# unpremultiply()

Transforms a floating-point 16-bit RGBA pixel buffer in-place from premultiplied alpha format to nonpremultiplied alpha format.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func unpremultiply()
```

Available when `Format` is `vImage.Interleaved16Fx4`.

## Discussion

This function divides the color values in each pixel `self` by the corresponding alpha value and copies the alpha value to the destination unchanged.

For example, the following code divides the RGB values `[0.125, 0.25, 0.5]` by the alpha value `0.5`:

```
let pixelValues = [0.125, 0.25, 0.5,
                   Float(0.5)].map {
    return vImage.Planar16F.makePixel($0)
}

let src = vImage.PixelBuffer(
    pixelValues: pixelValues,
    size: vImage.Size(width: 1, height: 1))

src.unpremultiply()

let result = src.array.map {
    return vImage.PlanarF.makePixel($0)
}

// Prints "[0.25, 0.5, 1.0, 0.5]".
print(result)
```

## See Also

### Unpremultiply

func unpremultiply(alpha: vImage.PixelBuffer&lt;Format>)

Transforms an 8-bit planar pixel buffer in-place from premultiplied alpha format to nonpremultiplied alpha format.

func unpremultiply(alpha: vImage.PixelBuffer&lt;Format>)

Transforms a 32-bit planar pixel buffer in-place from premultiplied alpha format to nonpremultiplied alpha format.

func unpremultiply(channelOrdering: vImage.ChannelOrdering)

Transforms an 8-bit ARGB or RGBA pixel buffer in-place from premultiplied alpha format to nonpremultiplied alpha format.

func unpremultiply(channelOrdering: vImage.ChannelOrdering)

Transforms an unsigned 16-bit ARGB or RGBA pixel buffer in-place from premultiplied alpha format to nonpremultiplied alpha format.

func unpremultiply(channelOrdering: vImage.ChannelOrdering)

Transforms a 32-bit ARGB or RGBA pixel buffer in-place from premultiplied alpha format to nonpremultiplied alpha format.

