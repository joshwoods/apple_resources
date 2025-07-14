

- MetalFX
- MTLFXTemporalScaler
-  jitterOffsetY 

Instance Property

# jitterOffsetY

The vertical component of the subpixel sampling coordinate you use to generate the color texture input.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+

``` source
var jitterOffsetY: Float { get set }
```

**Required**

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

var exposureTexture: (any MTLTexture)?

A texture that sets the exposure level for the color texture input.

**Required**

var preExposure: Float

The exposure value that you’ve already applied to your color texture input.

**Required**

