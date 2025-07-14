

- MetalKit
- MTKTextureLoader
- MTKTextureLoader.Option
-  textureStorageMode 

Type Property

# textureStorageMode

A key used to specify the storage mode for the texture.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
static let textureStorageMode: MTKTextureLoader.Option
```

## Discussion

The value for this key is an NSNumber object containing a MTLStorageMode value.

If this option is omitted, the texture is created with the default storage mode for Metal textures: MTLStorageMode.shared on iOS and tvOS, and MTLStorageMode.managed in macOS. Specifying the MTLStorageMode.private option causes the MTKTextureLoader object to submit work to the GPU on your behalf.

## See Also

### Specifying Resource Options

static let textureCPUCacheMode: MTKTextureLoader.Option

A key used to specify the CPU cache mode for the texture.

static let textureUsage: MTKTextureLoader.Option

A key used to specify the intended usage of the texture.

