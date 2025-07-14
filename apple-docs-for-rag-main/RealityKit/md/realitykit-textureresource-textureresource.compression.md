

- RealityKit
- TextureResource
-  TextureResource.Compression 

Structure

# TextureResource.Compression

The compression to apply when importing an image as a texture.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct Compression
```

## Overview

Compression allows varying levels of memory usage gains at the cost of image-quality reduction.

## Topics

### Specifying the compression settings

static var `default`: TextureResource.Compression

A texture you can create and export with lossy compression.

static var none: TextureResource.Compression

A texture you can create with no compression.

static func astc(blockSize: TextureResource.Compression.ASTCBlockSize, quality: TextureResource.Compression.ASTCQuality) -> TextureResource.Compression

Compresses the imported image with ASTC.

enum ASTCBlockSize

The compressed block size.

enum ASTCQuality

Selects the level of processing time allocated to achieve compression.

### Comparing compression settings

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

var hashValue: Int

The hash value.

### Operators

static func == (TextureResource.Compression, TextureResource.Compression) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

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

struct Format

The pixel format and encoding of a texture.

