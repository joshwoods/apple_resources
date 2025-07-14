

- RealityKit
- TextureResource
-  TextureResource.Dimensions2DArray 

Structure

# TextureResource.Dimensions2DArray

The dimensions of the 2D array texture.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct Dimensions2DArray
```

## Overview

This specifies the width, height, and length of the 2D array texture.

## Topics

### Creating the 2D array dimensions

static func dimensions(width: Int, height: Int, length: Int) -> TextureResource.Dimensions2DArray

Specifies the dimensions of the 2D array texture.

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

### Creating a 2D array texture resource

static func texture2DArray(slices: [CGImage], named: String?, options: TextureResource.CreateOptions) async throws -> TextureResource

Asynchronously creates a 2D texture array by generating it from images.

static func texture2DArray(slices: [CGImage], named: String?, options: TextureResource.CreateOptions) throws -> TextureResource

Synchronously creates a 2D texture array by generating it from images.

convenience init(dimensions: TextureResource.Dimensions2DArray, format: TextureResource.Format, contents: TextureResource.Contents) async throws

Asynchronously creates a 2D array texture resource from a pixel Metal buffer, or data.

convenience init(dimensions: TextureResource.Dimensions2DArray, format: TextureResource.Format, contents: TextureResource.Contents) throws

Synchronously creates a 2D array texture resource from a pixel Metal buffer, or data.

