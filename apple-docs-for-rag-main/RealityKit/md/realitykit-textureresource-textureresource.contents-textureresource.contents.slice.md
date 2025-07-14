

- RealityKit
- TextureResource
- TextureResource.Contents
-  TextureResource.Contents.Slice 

Structure

# TextureResource.Contents.Slice

An object that references the pixel data for a single slice of a mipmap.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct Slice
```

## Overview

2D array textures have `arrayLength` slices per mipmap, and cube textures have six slices per mipmap. 2D and 3D textures have a single slice per mipmap.

## Topics

### Creating a texture slice

static func slice(data: Data, bytesPerRow: Int) -> TextureResource.Contents.Slice

Specifies a single mipmap level slice of a texture resource with pixel data that RealityKit copies from a byte buffer.

static func slice(unsafeBuffer: any MTLBuffer, offset: Int, size: Int, bytesPerRow: Int) -> TextureResource.Contents.Slice

Specifies a single mipmap level slice of a texture resource with pixel data that RealityKit copies from a Metal buffer.

## Relationships

### Conforms To

- Sendable

## See Also

### Defining the content

struct MipmapLevel

An object that references the pixel data for a single mipmap of a texture.

