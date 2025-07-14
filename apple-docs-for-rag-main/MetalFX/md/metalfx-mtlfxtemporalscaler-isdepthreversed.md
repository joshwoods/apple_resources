

- MetalFX
- MTLFXTemporalScaler
-  isDepthReversed 

Instance Property

# isDepthReversed

A Boolean value that indicates whether the depth texture uses zero to represent the farthest distance.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+

``` source
var isDepthReversed: Bool { get set }
```

**Required**

## See Also

### Configuring the depth input

var depthTextureUsage: MTLTextureUsage

The minimal texture usage options that your app’s input depth texture must set to apply the temporal scaler.

**Required**

var depthTexture: (any MTLTexture)?

An input depth texture you set for the temporal scaler that supports the correct depth texture usage options.

**Required**

