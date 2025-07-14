

- Accelerate
- vImage
- vImage.BlendMode
-  vImage.BlendMode.lighten 

Case

# vImage.BlendMode.lighten

Sets each channel of the destination pixel as the lightest value for the corresponding channel of the two source layers

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
case lighten
```

## Discussion

The following image shows the result of compositing using the lighten blend mode:

The top-left quadrant in the result is white because no pixels in the bottom layer are brighter than the corresponding pixels in the top layer.

The bottom-left quadrant in the result looks washed out because the operation selects gray pixels from the top layer over corresponding dark pixels from the bottom layer.

## See Also

### Related Documentation

Compositing images with alpha blending

Combine two images by using alpha blending to create a single output.

### Enumeration Cases

case darken

Sets each channel of the destination pixel as the darkest value for the corresponding channel of the two source layers.

case multiply

Sets the destination pixel as the product of the corresponding source pixels.

case screen

Sets the destination pixel as the inverted product of the inverted corresponding source pixels.

