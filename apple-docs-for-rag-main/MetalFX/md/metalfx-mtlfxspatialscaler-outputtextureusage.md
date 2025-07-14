

- MetalFX
- MTLFXSpatialScaler
-  outputTextureUsage 

Instance Property

# outputTextureUsage

The minimal texture usage options that your app’s output texture must set to apply the spatial scaler.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var outputTextureUsage: MTLTextureUsage { get }
```

**Required**

## Discussion

The texture your app sets to the outputTexture property must use the same set (or a superset) of the MTLTextureUsage options in this property.

## See Also

### Configuring the image output

var outputTexture: (any MTLTexture)?

An output texture that supports the correct depth texture usage options.

**Required**

