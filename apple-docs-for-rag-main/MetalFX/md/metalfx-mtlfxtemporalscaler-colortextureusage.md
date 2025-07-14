

- MetalFX
- MTLFXTemporalScaler
-  colorTextureUsage 

Instance Property

# colorTextureUsage

The minimal texture usage options that your app’s input color texture must set to apply the temporal scaler.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+

``` source
var colorTextureUsage: MTLTextureUsage { get }
```

**Required**

## Discussion

The input texture you set to the colorTexture property must use the same set (or a superset) of the MTLTextureUsage options in this property.

## See Also

### Configuring the image input

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

var exposureTexture: (any MTLTexture)?

A texture that sets the exposure level for the color texture input.

**Required**

var preExposure: Float

The exposure value that you’ve already applied to your color texture input.

**Required**

