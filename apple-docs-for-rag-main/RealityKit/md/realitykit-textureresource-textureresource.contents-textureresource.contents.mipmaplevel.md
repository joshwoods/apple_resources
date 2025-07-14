

- RealityKit
- TextureResource
- TextureResource.Contents
-  TextureResource.Contents.MipmapLevel 

Structure

# TextureResource.Contents.MipmapLevel

An object that references the pixel data for a single mipmap of a texture.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
struct MipmapLevel
```

## Topics

### Creating a texture mipmap level

static func mip(data: Data, bytesPerRow: Int) -> TextureResource.Contents.MipmapLevel

Specifies a single mipmap level of a texture resource with pixel data that RealityKit copies from a byte buffer.

static func mip(data: Data, bytesPerRow: Int, bytesPerImage: Int) -> TextureResource.Contents.MipmapLevel

Specifies a multi-image mipmap level of a texture resource with pixel data that RealityKit copies from a byte buffer.

static func mip(slices: [TextureResource.Contents.Slice]) -> TextureResource.Contents.MipmapLevel

Specifies a single mipmap level of a 2D or 3D texture resource that slices provide.

static func mip(unsafeBuffer: any MTLBuffer, offset: Int, size: Int, bytesPerRow: Int) -> TextureResource.Contents.MipmapLevel

Specifies a single mipmap level of a texture resource with pixel data that RealityKit copies from a Metal buffer.

static func mip(unsafeBuffer: any MTLBuffer, offset: Int, size: Int, bytesPerRow: Int, bytesPerImage: Int) -> TextureResource.Contents.MipmapLevel

Specifies a multi-image mipmap level of a texture resource with pixel data that RealityKit copies from a Metal buffer.

## Relationships

### Conforms To

- Sendable

## See Also

### Defining the content

struct Slice

An object that references the pixel data for a single slice of a mipmap.

