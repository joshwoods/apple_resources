

- RealityKit
- TextureResource
-  TextureResource.Contents 

Structure

# TextureResource.Contents

An object that references the pixel data for each mipmap level of a texture.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
struct Contents
```

## Overview

Mipmaps are progressively smaller versions of the same texture image. Each level is half the size of the previous level, with a minimum size of 1 pixel in each dimension.

## Topics

### Creating the content

init(mipmapLevels: [TextureResource.Contents.MipmapLevel])

Creates a texture contents object from an array of mipmaps.

### Defining the content

struct MipmapLevel

An object that references the pixel data for a single mipmap of a texture.

struct Slice

An object that references the pixel data for a single slice of a mipmap.

## Relationships

### Conforms To

- Sendable

## See Also

### Creating a texture resource

convenience init(from: LowLevelTexture) throws

Synchronously creates a texture resource from a low-level texture.

convenience init(from: LowLevelTexture) async throws

Asynchronously creates a texture resource from a low-level texture.

struct Format

The pixel format and encoding of a texture.

struct Compression

The compression to apply when importing an image as a texture.

