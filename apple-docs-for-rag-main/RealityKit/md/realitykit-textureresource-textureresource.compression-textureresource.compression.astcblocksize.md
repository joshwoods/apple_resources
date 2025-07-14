

- RealityKit
- TextureResource
- TextureResource.Compression
-  TextureResource.Compression.ASTCBlockSize 

Enumeration

# TextureResource.Compression.ASTCBlockSize

The compressed block size.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
enum ASTCBlockSize
```

## Overview

Note

RealityKit stores block pixel data in groups of 128 bits. For instance, a `block4x4` bits per pixel is 128/(4\*4) = 8 bit per pixel.

## Topics

### Compression block sizes

case block4x4

case block5x4

case block5x5

case block6x5

case block6x6

case block8x5

case block8x6

case block8x8

case block10x10

case block10x5

case block10x6

case block10x8

case block12x10

case block12x12

### Comparing compression block sizes

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

var hashValue: Int

The hash value.

### Operators

static func == (TextureResource.Compression.ASTCBlockSize, TextureResource.Compression.ASTCBlockSize) -> Bool

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

enum ASTCQuality

Selects the level of processing time allocated to achieve compression.

