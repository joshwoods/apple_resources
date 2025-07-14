

- MetalKit
- MTKTextureLoader
-  MTKTextureLoader.CubeLayout 

Structure

# MTKTextureLoader.CubeLayout

Options for specifying how cube texture data is arranged in the source image.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
struct CubeLayout
```

## Topics

### Creating Cube Texture Layout Options

init(rawValue: String)

Creates a cube layout option from a raw string value.

### Specifying Cube Texture Layout Options

static let vertical: MTKTextureLoader.CubeLayout

Specifies that the source 2D image is a vertical arrangement of six cube faces.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Specifying Cube Layout

static let cubeLayout: MTKTextureLoader.Option

A key used to specify how cube texture data is arranged in the source image.

