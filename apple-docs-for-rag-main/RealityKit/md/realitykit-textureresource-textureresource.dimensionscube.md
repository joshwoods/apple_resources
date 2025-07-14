

- RealityKit
- TextureResource
-  TextureResource.DimensionsCube 

Structure

# TextureResource.DimensionsCube

The dimensions of the cube texture.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct DimensionsCube
```

## Overview

This specifies the face size of the cube texture.

## Topics

### Creating the cube dimensions

static func dimensions(faceSize: Int) -> TextureResource.DimensionsCube

Specifies the dimensions of the cube texture.

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

### Creating a cube texture resource

convenience init(cubeFromEquirectangular: CGImage, named: String?, quality: TextureResource.SamplingQuality, faceSize: Int?, options: TextureResource.CreateOptions) throws

Synchronously creates a cube texture resource from an equirectangular image.

convenience init(cubeFromEquirectangular: CGImage, named: String?, quality: TextureResource.SamplingQuality, faceSize: Int?, options: TextureResource.CreateOptions) async throws

Asynchronously creates a cube texture resource from an equirectangular image.

convenience init(cubeFromImage: CGImage, named: String?, options: TextureResource.CreateOptions) throws

Synchronously creates a cube texture resource from a 2D image of cube faces.

convenience init(cubeFromImage: CGImage, named: String?, options: TextureResource.CreateOptions) async throws

Asynchronously creates a cube texture resource from a 2D image of cube faces.

static func cube(slices: [CGImage], named: String?, options: TextureResource.CreateOptions) async throws -> TextureResource

Asynchronously creates a cube texture resource from face images.

static func cube(slices: [CGImage], named: String?, options: TextureResource.CreateOptions) throws -> TextureResource

Synchronously creates a cube texture resource from face images.

convenience init(dimensions: TextureResource.DimensionsCube, format: TextureResource.Format, contents: TextureResource.Contents) throws

Synchronously creates a cube texture resource from a pixel Metal buffer, or data.

convenience init(dimensions: TextureResource.DimensionsCube, format: TextureResource.Format, contents: TextureResource.Contents) async throws

Asynchronously creates a cube texture resource from a pixel Metal buffer, or data.

