

- MetalFX
- MTLFXTemporalScaler
-  motionVectorScaleY 

Instance Property

# motionVectorScaleY

The vertical scale factor the temporal scaler applies to the input motion texture.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+

``` source
var motionVectorScaleY: Float { get set }
```

**Required**

## Discussion

The scaler converts the vertical component of each value in motionTexture into fragment (pixel) coordinates by multiplying it by this property’s value.

## See Also

### Configuring the motion input

var motionTextureUsage: MTLTextureUsage

The minimal texture usage options that your app’s input motion texture must set to apply the temporal scaler.

**Required**

var motionTexture: (any MTLTexture)?

An input motion texture you set for the temporal scaler that supports the correct motion texture usage options.

**Required**

var motionVectorScaleX: Float

The horizontal scale factor the temporal scaler applies to the input motion texture.

**Required**

