

- RealityKit
- TextureResource
-  TextureResource.Semantic 

Enumeration

# TextureResource.Semantic

An object for specifying the intended use of a texture.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
enum Semantic
```

## Overview

RealityKit uses image textures to transmit different types of data Metal shaders. For example, it uses textures to send RGB images with the base color of the entity, to send grayscale images holding roughness and metallic information, and to send surface normals for doing lighting calculations.

This object specifies the intended use of the texture by an individual property.

## Topics

### Specifying intended use

case raw

Use the texture unmodified.

case color

Use the texture to store colors data.

case hdrColor

Use the texture to store a high-dynamic range image.

case normal

Use the texture to store surface normals.

case scalar

Use the texture to store a single value in each pixel.

### Comparing enumeration values

var hashValue: Int

The hash value.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

static func == (TextureResource.Semantic, TextureResource.Semantic) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Texture resources

class TextureResource

A representation of a texture.

struct CreateOptions

An object that holds texture resource creation options.

typealias SamplingQuality

An object for controlling the texture-sampling quality.

enum MipmapsMode

An enumeration for specifying how to allocate and generate mipmaps for a texture.

