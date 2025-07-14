

- MetalFX
- MTLFXTemporalScaler
-  exposureTexture 

Instance Property

# exposureTexture

A texture that sets the exposure level for the color texture input.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+

``` source
var exposureTexture: (any MTLTexture)? { get set }
```

**Required**

## Discussion

The property is a texture (unlike preExposure) so that the GPU can directly modify the exposure level for each frame at runtime.

Tip

For best results, set this property to a texture with a single MTLPixelFormat.r16Float element.

The temporal scaler uses only the red component of the texture’s first value, at location (0, 0), as the exposure factor. If the property is `nil`, the default exposure factor is `1.0`.

Note

The temporal scaler ignores this property if you create it with a descriptor that has its isAutoExposureEnabled property set to true.

## See Also

### Configuring the image input

var colorTextureUsage: MTLTextureUsage

The minimal texture usage options that your app’s input color texture must set to apply the temporal scaler.

**Required**

var colorTexture: (any MTLTexture)?

An input color texture you set for the temporal scaler that supports the correct color texture usage options.

**Required**

var inputContentWidth: Int

The width, in pixels, of the region within the color texture the temporal scaler uses as its input.

**Required**

var inputContentHeight: Int

The height, in pixels, of the region within the color texture the temporal scaler uses as its input.

**Required**

var jitterOffsetX: Float

The horizontal component of the subpixel sampling coordinate you use to generate the color texture input.

**Required**

var jitterOffsetY: Float

The vertical component of the subpixel sampling coordinate you use to generate the color texture input.

**Required**

var preExposure: Float

The exposure value that you’ve already applied to your color texture input.

**Required**

