

- Accelerate
- vImage
- vImage.PixelBuffer
-  alphaComposite(\_:topLayer:destination:) 

Instance Method

# alphaComposite(\_:topLayer:destination:)

Performs alpha compositing of two 4-channel interleaved ARGB 8-bit pixel buffers using the specified composite mode.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func alphaComposite(
    _ compositeMode: vImage.CompositeMode,
    topLayer: vImage.PixelBuffer,
    destination: vImage.PixelBuffer
)
```

Available when `Format` is `vImage.Interleaved8x4`.

## Parameters 

`compositeMode`  

The composite mode.

`topLayer`  

The composite top layer.

`destination`  

The destination pixel buffer.

## Discussion

This function treats `self` as the bottom layer and both pixel buffers must have alpha as their first channel.

## See Also

### Related Documentation

Compositing images with alpha blending

Combine two images by using alpha blending to create a single output.

### Alpha compositing

func alphaComposite(vImage.CompositeMode&lt;Pixel_F>, topLayer: vImage.PixelBuffer&lt;Format>, destination: vImage.PixelBuffer&lt;Format>)

Performs alpha compositing of two 4-channel interleaved ARGB 32-bit pixel buffers using the specified composite mode.

enum CompositeMode

Constants that specify whether the format of layers is premultiplied or nonpremultiplied.

