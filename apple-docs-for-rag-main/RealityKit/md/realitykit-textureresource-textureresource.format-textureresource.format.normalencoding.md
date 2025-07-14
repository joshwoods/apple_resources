

- RealityKit
- TextureResource
- TextureResource.Format
-  TextureResource.Format.NormalEncoding 

Enumeration

# TextureResource.Format.NormalEncoding

A profile that specifies the interpretation of pixel values as a normal.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
enum NormalEncoding
```

## Topics

### Normal profiles

case wy

A normal map with the X and Y components of a surface normal in the tangent space of the surface that RealityKit encodes in the alpha and green channels of a texture.

case xy

A normal map with the X and Y components of a surface normal in the tangent space of the surface that RealityKit encodes in the red and green channels of a texture.

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

### Defining the format profile

enum ColorSpace

A profile that specifies the interpretation of pixel values as a color.

