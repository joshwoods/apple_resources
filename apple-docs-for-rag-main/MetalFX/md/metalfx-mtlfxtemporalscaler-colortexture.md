

- MetalFX
- MTLFXTemporalScaler
-  colorTexture 

Instance Property

# colorTexture

An input color texture you set for the temporal scaler that supports the correct color texture usage options.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+

``` source
var colorTexture: (any MTLTexture)? { get set }
```

**Required**

## Discussion

The texture you set to this property must meet the following requirements:

- The texture’s usage property must use the same MTLTextureUsage options as (or be a superset of) the temporal scaling effect’s colorTextureUsage property.

- The texture’s dimensions must be equal to the inputWidth and inputHeight properties.

## See Also

### Configuring the image input

var colorTextureUsage: MTLTextureUsage

The minimal texture usage options that your app’s input color texture must set to apply the temporal scaler.

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

