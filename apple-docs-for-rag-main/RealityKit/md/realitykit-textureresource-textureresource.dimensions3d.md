

- RealityKit
- TextureResource
-  TextureResource.Dimensions3D 

Structure

# TextureResource.Dimensions3D

The dimensions of the 3D texture.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct Dimensions3D
```

## Overview

This specifies the width, height, and depth of the 3D texture

## Topics

### Creating the 3D dimensions

static func dimensions(width: Int, height: Int, depth: Int) -> TextureResource.Dimensions3D

Specifies the dimensions of the 3D texture.

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

### Creating a 3D texture resource

static func texture3D(slices: [CGImage], named: String?, options: TextureResource.CreateOptions) async throws -> TextureResource

Asynchronously creates a 3D texture by generating it from images.

static func texture3D(slices: [CGImage], named: String?, options: TextureResource.CreateOptions) throws -> TextureResource

Synchronously creates a 3D texture by generating it from images.

convenience init(dimensions: TextureResource.Dimensions3D, format: TextureResource.Format, contents: TextureResource.Contents) throws

Synchronously creates a 3D texture resource from a pixel Metal buffer, or data.

convenience init(dimensions: TextureResource.Dimensions3D, format: TextureResource.Format, contents: TextureResource.Contents) async throws

Asynchronously creates a 3D texture resource from a pixel Metal buffer, or data.

