

- MetalKit
- MTKTextureLoader
-  MTKTextureLoader.Option 

Structure

# MTKTextureLoader.Option

Keys and values used to specify loading options.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
struct Option
```

## Topics

### Creating Texture Loading Options

init(rawValue: String)

Creates a texture loader option from a raw string value.

### Specifying Mipmap Options

static let allocateMipmaps: MTKTextureLoader.Option

A key used to specify whether the texture loader should allocate memory for mipmaps in the texture.

static let generateMipmaps: MTKTextureLoader.Option

A key used to specify whether the texture loader should generate mipmaps for the texture.

### Specifying Resource Options

static let textureCPUCacheMode: MTKTextureLoader.Option

A key used to specify the CPU cache mode for the texture.

static let textureStorageMode: MTKTextureLoader.Option

A key used to specify the storage mode for the texture.

static let textureUsage: MTKTextureLoader.Option

A key used to specify the intended usage of the texture.

### Specifying Origin Information

static let origin: MTKTextureLoader.Option

A key used to specify when to flip the pixel coordinates of the texture.

struct Origin

Options for specifying when to flip the pixel coordinates of the texture.

### Specifying Cube Layout

static let cubeLayout: MTKTextureLoader.Option

A key used to specify how cube texture data is arranged in the source image.

struct CubeLayout

Options for specifying how cube texture data is arranged in the source image.

### Specifying sRGB Options

static let SRGB: MTKTextureLoader.Option

A key used to specify whether the texture data is stored as sRGB image data.

### Type Properties

static let loadAsArray: MTKTextureLoader.Option

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

