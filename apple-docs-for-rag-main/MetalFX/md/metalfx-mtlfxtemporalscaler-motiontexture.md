

- MetalFX
- MTLFXTemporalScaler
-  motionTexture 

Instance Property

# motionTexture

An input motion texture you set for the temporal scaler that supports the correct motion texture usage options.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+

``` source
var motionTexture: (any MTLTexture)? { get set }
```

**Required**

## Discussion

The texture you set to this property must meet the following requirements:

- The texture’s usage property must use the same MTLTextureUsage options as (or be a superset of) the temporal scaling effect’s motionTextureUsage property.

- The texture’s dimensions must be equal to the inputWidth and inputHeight properties.

## See Also

### Configuring the motion input

var motionTextureUsage: MTLTextureUsage

The minimal texture usage options that your app’s input motion texture must set to apply the temporal scaler.

**Required**

var motionVectorScaleX: Float

The horizontal scale factor the temporal scaler applies to the input motion texture.

**Required**

var motionVectorScaleY: Float

The vertical scale factor the temporal scaler applies to the input motion texture.

**Required**

