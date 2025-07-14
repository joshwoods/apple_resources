

- RealityKit
- TextureResource
-  TextureResource.Format 

Structure

# TextureResource.Format

The pixel format and encoding of a texture.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
struct Format
```

## Overview

The texture’s format controls the sampling and conversions (if any) to use when rendering with that texture.

## Topics

### Creating the format

static func color(TextureResource.Format.ColorSpace, pixelFormat: MTLPixelFormat) -> TextureResource.Format

Indicates that a texture contains color data to interpret in a specific color space.

static func normal(TextureResource.Format.NormalEncoding, pixelFormat: MTLPixelFormat) -> TextureResource.Format

Indicates that a texture is a normal map.

static func raw(pixelFormat: MTLPixelFormat) -> TextureResource.Format

Indicates a texture for unmodified use by a shader.

### Defining the format profile

enum ColorSpace

A profile that specifies the interpretation of pixel values as a color.

enum NormalEncoding

A profile that specifies the interpretation of pixel values as a normal.

### Default Implementations

Equatable Implementations

Hashable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Creating a texture resource

convenience init(from: LowLevelTexture) throws

Synchronously creates a texture resource from a low-level texture.

convenience init(from: LowLevelTexture) async throws

Asynchronously creates a texture resource from a low-level texture.

struct Contents

An object that references the pixel data for each mipmap level of a texture.

struct Compression

The compression to apply when importing an image as a texture.

