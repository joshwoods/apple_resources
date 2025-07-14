

- RealityKit
- PhysicallyBasedMaterial
-  PhysicallyBasedMaterial.Opacity 

Structure

# PhysicallyBasedMaterial.Opacity

An object that defines the opacity of an entity.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
struct Opacity
```

## Topics

### Creating an opacity object

init(floatLiteral: Float)

Creates an opacity object using a single value.

init(scale: Float, texture: PhysicallyBasedMaterial.Texture?)

Creates an opacity object using a single value or a texture.

init(CustomMaterial.Opacity)

Creates an opacity object using a custom material’s opacity property.

### Accessing opacity values

var texture: PhysicallyBasedMaterial.Texture?

The amount of opacity specified using a UV-mapped image.

static var textureSemantic: TextureResource.Semantic

The intended use of the object’s texture property.

var scale: Float

var opacityThreshold: Float?

A threshold below which RealityKit ignores opacity.

typealias FloatLiteralType

A type that represents a floating-point literal.

## Relationships

### Conforms To

- ExpressibleByFloatLiteral

## See Also

### Specifying opacity

case opaque

An opaque surface.

case transparent(opacity: PhysicallyBasedMaterial.Opacity)

A surface that’s transparent.

var opacityThreshold: Float?

A threshold below which RealityKit ignores opacity.

