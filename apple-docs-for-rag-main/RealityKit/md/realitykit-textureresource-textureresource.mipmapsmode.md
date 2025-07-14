

- RealityKit
- TextureResource
-  TextureResource.MipmapsMode 

Enumeration

# TextureResource.MipmapsMode

An enumeration for specifying how to allocate and generate mipmaps for a texture.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
enum MipmapsMode
```

## Topics

### Specifying allocation and generation

case none

Do not allocate mipmaps for the texture resource.

case allocateAll

Allocate memory for all mipmaps, but don’t generate them.

case allocateAndGenerateAll

Allocate and generate all mipmaps for the texture resource.

### Comparing enumeration values

var hashValue: Int

The hash value.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

static func == (TextureResource.MipmapsMode, TextureResource.MipmapsMode) -> Bool

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

enum Semantic

An object for specifying the intended use of a texture.

