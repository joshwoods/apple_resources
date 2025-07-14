

- MetalKit
- MTKTextureLoader
- MTKTextureLoader.Option
-  textureUsage 

Type Property

# textureUsage

A key used to specify the intended usage of the texture.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
static let textureUsage: MTKTextureLoader.Option
```

## Discussion

The value for this key is an NSNumber object containing a MTLTextureUsage value.

If this key is not specified, the default value is determined by the default usage value of the MTLTextureDescriptor class. When you create a texture, determine the specific ways in which it will be used, and set the texture usage to contain just those options. Do not set usage options that you don’t intend to use. Metal uses these flags to determine how the texture is allocated and configured; setting them correctly can significantly improve your app’s performance..

## See Also

### Specifying Resource Options

static let textureCPUCacheMode: MTKTextureLoader.Option

A key used to specify the CPU cache mode for the texture.

static let textureStorageMode: MTKTextureLoader.Option

A key used to specify the storage mode for the texture.

