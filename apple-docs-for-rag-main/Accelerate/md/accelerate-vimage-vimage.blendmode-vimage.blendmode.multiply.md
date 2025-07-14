

- Accelerate
- vImage
- vImage.BlendMode
-  vImage.BlendMode.multiply 

Case

# vImage.BlendMode.multiply

Sets the destination pixel as the product of the corresponding source pixels.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
case multiply
```

## Discussion

The following image shows the result of compositing using the multiply blend mode:

The bottom-right quadrant in the result is black because the operation multiplies each bottom-layer pixel value by `0.0` from the top layer.

The top-left quadrant in the result is identical to the corresponding quadrant in the bottom layer because the operation multiplies each bottom-layer pixel value by `1.0`.

The top-right quadrant in the result is darker than the corresponding quadrant in the bottom layer. In this quadrant, the top-layer and bottom-layer pixel values are identical. For example, if the source pixel value is 0.5, the destination pixel value is `0.25`:

```
dest = 0.5 * 0.5 // dest = 0.25
```

## See Also

### Related Documentation

Compositing images with alpha blending

Combine two images by using alpha blending to create a single output.

### Enumeration Cases

case darken

Sets each channel of the destination pixel as the darkest value for the corresponding channel of the two source layers.

case lighten

Sets each channel of the destination pixel as the lightest value for the corresponding channel of the two source layers

case screen

Sets the destination pixel as the inverted product of the inverted corresponding source pixels.

