

- RealityKit
- TextureResource
- TextureResource.Compression
-  TextureResource.Compression.ASTCQuality 

Enumeration

# TextureResource.Compression.ASTCQuality

Selects the level of processing time allocated to achieve compression.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
enum ASTCQuality
```

## Overview

Important

Given its processing cost, runtime compression isn’t recommended for interactive apps, as opposed to loading `.reality` files or `.ktx` precompressed textures. Higher quality levels are recommended for pipelines assembling scenes you intend to export to `.reality` files.

## Topics

### Compression qualities

case exhaustive

Compresses optimally, achieving minor gains over high-level compression at the cost of much longer processing times.

case fast

Compresses as fast as possible.

case high

Compresses with a focus on quality, reaching close to optimal quality while still spending much less time than exhaustive-level compression.

case normal

Compresses with a good balance between quality and processing time.

### Comparing compression quality

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

var hashValue: Int

The hash value.

### Operators

static func == (TextureResource.Compression.ASTCQuality, TextureResource.Compression.ASTCQuality) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Specifying the compression settings

static var `default`: TextureResource.Compression

A texture you can create and export with lossy compression.

static var none: TextureResource.Compression

A texture you can create with no compression.

static func astc(blockSize: TextureResource.Compression.ASTCBlockSize, quality: TextureResource.Compression.ASTCQuality) -> TextureResource.Compression

Compresses the imported image with ASTC.

enum ASTCBlockSize

The compressed block size.

