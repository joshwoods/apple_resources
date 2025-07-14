

- RealityKit
- MaterialParameters
-  MaterialParameters.Texture 

Structure

# MaterialParameters.Texture

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
struct Texture
```

## Topics

### Structures

struct Sampler

### Initializers

init(TextureResource)

init(TextureResource, sampler: MaterialParameters.Texture.Sampler)

### Instance Properties

var resource: TextureResource

var sampler: MaterialParameters.Texture.Sampler

var swizzle: MTLTextureSwizzleChannels

Channel swizzle to use when RealityKit reads or samples from the texture.

var uvIndex: Int

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable

