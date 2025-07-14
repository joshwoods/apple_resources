

- RealityKit
- TextureResource
-  TextureResource.CreateOptions 

Structure

# TextureResource.CreateOptions

An object that holds texture resource creation options.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
struct CreateOptions
```

## Topics

### Texture resource initializers

init(semantic: TextureResource.Semantic?, mipmapsMode: TextureResource.MipmapsMode)

Creates a texture creation options structure.

### Texture resource creation options

var mipmapsMode: TextureResource.MipmapsMode

Whether the texture resource automatically generates mipmaps.

var semantic: TextureResource.Semantic?

The intended use of the texture.

### Initializers

init(semantic: TextureResource.Semantic?, compression: TextureResource.Compression, mipmapsMode: TextureResource.MipmapsMode)

Creates a texture creation options structure.

### Instance Properties

var compression: TextureResource.Compression

## See Also

### Texture resources

class TextureResource

A representation of a texture.

typealias SamplingQuality

An object for controlling the texture-sampling quality.

enum MipmapsMode

An enumeration for specifying how to allocate and generate mipmaps for a texture.

enum Semantic

An object for specifying the intended use of a texture.

