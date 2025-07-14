

- MetalFX
- MTLFXTemporalScaler
-  motionTextureUsage 

Instance Property

# motionTextureUsage

The minimal texture usage options that your app’s input motion texture must set to apply the temporal scaler.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+

``` source
var motionTextureUsage: MTLTextureUsage { get }
```

**Required**

## Discussion

The input texture you set to the motionTexture property must use the same set (or a superset) of the MTLTextureUsage options in this property.

## See Also

### Configuring the motion input

var motionTexture: (any MTLTexture)?

An input motion texture you set for the temporal scaler that supports the correct motion texture usage options.

**Required**

var motionVectorScaleX: Float

The horizontal scale factor the temporal scaler applies to the input motion texture.

**Required**

var motionVectorScaleY: Float

The vertical scale factor the temporal scaler applies to the input motion texture.

**Required**

