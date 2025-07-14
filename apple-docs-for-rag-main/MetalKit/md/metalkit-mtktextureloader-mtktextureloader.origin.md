

- MetalKit
- MTKTextureLoader
-  MTKTextureLoader.Origin 

Structure

# MTKTextureLoader.Origin

Options for specifying when to flip the pixel coordinates of the texture.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
struct Origin
```

## Topics

### Creating Texture Origin Options

init(rawValue: String)

Creates a texture origin option from a raw string value.

### Specifying Texture Origin Options

static let topLeft: MTKTextureLoader.Origin

An option for specifying images that should be flipped only to put their origin in the top-left corner.

static let bottomLeft: MTKTextureLoader.Origin

An option for specifying images that should be flipped only to put their origin in the bottom-left corner.

static let flippedVertically: MTKTextureLoader.Origin

An option that specifies that images should always be flipped.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Specifying Origin Information

static let origin: MTKTextureLoader.Option

A key used to specify when to flip the pixel coordinates of the texture.

