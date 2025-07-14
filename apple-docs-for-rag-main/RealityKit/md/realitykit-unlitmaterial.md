

- RealityKit
-  UnlitMaterial 

Structure

# UnlitMaterial

A material that doesn’t respond to lights in the scene.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
struct UnlitMaterial
```

## Mentioned in 

Modifying RealityKit rendering using custom materials

## Overview

`UnlitMaterial` materials do not respond to virtual or real lighting.

Add an `UnlitMaterial` to a model by setting it as one of the materials in a ModelComponent.

```
let unlitMaterial = UnlitMaterial(color: .red)
let model = ModelComponent(
    mesh: .generateBox(size: 1),
    materials: [unlitMaterial]
)
redBoxEntity.components.set(model)
```

For example, a SimpleMaterial on the left, and an `UnlitMaterial` on the right:

| SimpleMaterial | `UnlitMaterial` |
|----|----|
|  |  |

Note

The blending mode of `UnlitMaterial` materials should be configured explicitly with the blending property for transparent or translucent surfaces. The `opaque` mode is used when unset.

## Topics

### Creating an unlit material

init()

Creates an unlit material.

init(color: UIColor)

Creates an unlit material with the given base color.

init(color: NSColor)

Creates an unlit material with the given base color.

init(applyPostProcessToneMap: Bool)

init(color: NSColor, applyPostProcessToneMap: Bool)

init(color: UIColor, applyPostProcessToneMap: Bool)

init(program: UnlitMaterial.Program)

init(texture: TextureResource)

Creates a new unlit material with the provided color texture.

### Configuring base color

var color: UnlitMaterial.BaseColor

The material’s base color.

var baseColor: MaterialColorParameter

The base color of the material.

Deprecated

### Tinting an unlit material

var tintColor: NSColor

A tint color applied to the base color.

Deprecated

var tintColor: UIColor

A tint color applied to the base color.

Deprecated

### Controlling opacity

var opacityThreshold: Float?

A threshold below which RealityKit ignores opacity.

var blending: UnlitMaterial.Blending

The transparency options for the material.

### Classes

class Program

An object that represents the backing shader compilation required for unlit materials.

### Instance Properties

var faceCulling: UnlitMaterial.FaceCulling

var program: UnlitMaterial.Program

var readsDepth: Bool

A boolean value that determines whether this material performs the depth test by reading RealityKit’s depth buffer.

var secondaryTextureCoordinateTransform: UnlitMaterial.TextureCoordinateTransform

A two-dimensional transformation to apply to the entity’s secondary texture coordinates.

var textureCoordinateTransform: UnlitMaterial.TextureCoordinateTransform

A two-dimensional transformation to apply to the entity’s primary texture coordinates.

var triangleFillMode: UnlitMaterial.TriangleFillMode

The object that controls how RealityKit draws triangles.

var writesDepth: Bool

A boolean value that determines whether this material writes its depth into RealityKit’s depth buffer.

### Type Aliases

typealias BaseColor

The type used to represent base color.

typealias Blending

The type used to represent opacity information.

typealias FaceCulling

An alias for the cull mode object that’s appropriate for this material class.

typealias Texture

The type used to represent textures.

typealias TextureCoordinateTransform

An alias for the texture coordinate transform that’s appropriate for this material class.

typealias TriangleFillMode

### Default Implementations

Material Implementations

## Relationships

### Conforms To

- Material

## See Also

### Unlit materials

typealias BaseColor

The type used to represent base color.

typealias Blending

The type used to represent opacity information.

typealias Texture

The type used to represent textures.

typealias Parameters

The parameter type that custom materials uses for properties the framework passes to shader functions.

typealias FaceCulling

An alias for the cull mode object that’s appropriate for this material class.

typealias TextureCoordinateTransform

An alias for the texture coordinate transform that’s appropriate for this material class.

typealias TriangleFillMode

