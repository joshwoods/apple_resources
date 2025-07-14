

- RealityKit
- TextureResource
-  init(from:) 

Initializer

# init(from:)

Asynchronously creates a texture resource from a low-level texture.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor @preconcurrency
convenience init(from texture: LowLevelTexture) async throws
```

## Parameters 

`texture`  

The texture data that defines the resource.

## See Also

### Creating a texture resource

convenience init(from: LowLevelTexture) throws

Synchronously creates a texture resource from a low-level texture.

struct Contents

An object that references the pixel data for each mipmap level of a texture.

struct Format

The pixel format and encoding of a texture.

struct Compression

The compression to apply when importing an image as a texture.

