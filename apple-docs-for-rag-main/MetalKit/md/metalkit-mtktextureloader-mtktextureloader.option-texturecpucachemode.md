

- MetalKit
- MTKTextureLoader
- MTKTextureLoader.Option
-  textureCPUCacheMode 

Type Property

# textureCPUCacheMode

A key used to specify the CPU cache mode for the texture.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
static let textureCPUCacheMode: MTKTextureLoader.Option
```

## Discussion

The value for this key is an NSNumber object containing a MTLCPUCacheMode value.

If this key is not specified, the default value is the value associated with MTLCPUCacheMode.defaultCache.

## See Also

### Specifying Resource Options

static let textureStorageMode: MTKTextureLoader.Option

A key used to specify the storage mode for the texture.

static let textureUsage: MTKTextureLoader.Option

A key used to specify the intended usage of the texture.

