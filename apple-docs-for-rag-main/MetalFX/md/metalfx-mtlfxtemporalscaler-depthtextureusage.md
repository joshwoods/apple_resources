

- MetalFX
- MTLFXTemporalScaler
-  depthTextureUsage 

Instance Property

# depthTextureUsage

The minimal texture usage options that your app’s input depth texture must set to apply the temporal scaler.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+

``` source
var depthTextureUsage: MTLTextureUsage { get }
```

**Required**

## Discussion

The input texture you set to the depthTexture property must use the same set (or a superset) of the MTLTextureUsage options in this property.

## See Also

### Configuring the depth input

var depthTexture: (any MTLTexture)?

An input depth texture you set for the temporal scaler that supports the correct depth texture usage options.

**Required**

var isDepthReversed: Bool

A Boolean value that indicates whether the depth texture uses zero to represent the farthest distance.

**Required**

