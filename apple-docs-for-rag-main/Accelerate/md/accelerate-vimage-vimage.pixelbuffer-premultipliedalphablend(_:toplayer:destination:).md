

- Accelerate
- vImage
- vImage.PixelBuffer
-  premultipliedAlphaBlend(\_:topLayer:destination:) 

Instance Method

# premultipliedAlphaBlend(\_:topLayer:destination:)

Performs alpha compositing of two 4-channel interleaved RGBA 8-bit pixel buffers using the specified blend mode to produce a premultiplied result.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func premultipliedAlphaBlend(
    _ blendMode: vImage.BlendMode,
    topLayer: vImage.PixelBuffer,
    destination: vImage.PixelBuffer
)
```

Available when `Format` is `vImage.Interleaved8x4`.

## Parameters 

`blendMode`  

The blend mode.

`topLayer`  

The blend top layer.

`destination`  

The destination pixel buffer.

## Discussion

This function treats `self` as the bottom layer and both pixel buffers must have alpha as their last channel.

## See Also

### Related Documentation

Compositing images with alpha blending

Combine two images by using alpha blending to create a single output.

### Alpha blending

enum BlendMode

Constants that specify an alpha blending mode.

