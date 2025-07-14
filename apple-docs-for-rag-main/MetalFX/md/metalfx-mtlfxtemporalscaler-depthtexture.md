

- MetalFX
- MTLFXTemporalScaler
-  depthTexture 

Instance Property

# depthTexture

An input depth texture you set for the temporal scaler that supports the correct depth texture usage options.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+

``` source
var depthTexture: (any MTLTexture)? { get set }
```

**Required**

## Discussion

The texture you set to this property must meet the following requirements:

- The texture’s usage property must use the same MTLTextureUsage options as (or be a superset of) the temporal scaling effect’s depthTextureUsage property.

- The texture’s dimensions must be equal to the inputWidth and inputHeight properties.

## See Also

### Configuring the depth input

var depthTextureUsage: MTLTextureUsage

The minimal texture usage options that your app’s input depth texture must set to apply the temporal scaler.

**Required**

var isDepthReversed: Bool

A Boolean value that indicates whether the depth texture uses zero to represent the farthest distance.

**Required**

