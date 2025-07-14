

- RealityKit
- TextureResource
-  TextureResource.Dimensions2D 

Structure

# TextureResource.Dimensions2D

The dimensions of a 2D texture.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
struct Dimensions2D
```

## Overview

This specifies the width and height of a 2D texture.

## Topics

### Creating the 2D dimensions

static func dimensions(width: Int, height: Int) -> TextureResource.Dimensions2D

Specifies the dimensions of the 2D texture.

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

### Creating a 2D texture resource

convenience init(image: CGImage, withName: String?, options: TextureResource.CreateOptions) async throws

Asynchronously creates a texture resource from an in-memory Core Graphics image.

convenience init(image: CGImage, withName: String?, options: TextureResource.CreateOptions) throws

Synchronously creates a texture resource from an in-memory Core Graphics image.

convenience init(dimensions: TextureResource.Dimensions2D, format: TextureResource.Format, contents: TextureResource.Contents) throws

Synchronously creates a 2D texture resource from a pixel Metal buffer, or data.

convenience init(dimensions: TextureResource.Dimensions2D, format: TextureResource.Format, contents: TextureResource.Contents) async throws

Asynchronously creates a 2D texture resource from a pixel Metal buffer, or data.

