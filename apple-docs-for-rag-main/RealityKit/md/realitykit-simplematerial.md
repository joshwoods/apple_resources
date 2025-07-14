

- RealityKit
-  SimpleMaterial 

Structure

# SimpleMaterial

A basic material that responds to lights in the scene.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
struct SimpleMaterial
```

## Mentioned in 

Adding procedural assets to a scene

## Overview

`SimpleMaterial` responds to both real and virtual lighting to enhance realism.

Add a `SimpleMaterial` to a model by setting it as one of the materials in a ModelComponent.

```
let simpleMaterial = SimpleMaterial(
    color: .red, isMetallic: false
)
let model = ModelComponent(
    mesh: .generateBox(size: 1),
    materials: [simpleMaterial]
)
redBoxEntity.components.set(model)
```

For example, a red `SimpleMaterial` that is not metallic, and one that is metallic:

| Not metallic | Metallic |
|----|----|
|  |  |

## Topics

### Creating a simple material

init()

Creates a simple material.

init(color: SimpleMaterial.Color, roughness: MaterialScalarParameter, isMetallic: Bool)

Creates a simple material with specific characteristics in macOS.

init(color: SimpleMaterial.Color, roughness: MaterialScalarParameter, isMetallic: Bool)

Creates a simple material with specific characteristics in macOS.

### Characterizing a material

var color: SimpleMaterial.BaseColor

The material’s color.

var baseColor: MaterialColorParameter

The base color of the material.

Deprecated

typealias BaseColor

The type used to represent base color.

var tintColor: UIColor

A tint color applied to the base color in macOS.

Deprecated

var tintColor: NSColor

A tint color applied to the base color in macOS.

Deprecated

typealias Texture

The type used to represent textures.

var metallic: MaterialScalarParameter

A value that you set to control whether the material has a metallic look.

var roughness: MaterialScalarParameter

The roughness of the material.

typealias Parameters

The parameter type that custom materials uses for properties the framework passes to shader functions.

### Instance Properties

var faceCulling: SimpleMaterial.FaceCulling

A process in which the system specifies polygons to remove before rendering a mesh using this material.

var readsDepth: Bool

A boolean value that determines whether this material performs the depth test by reading RealityKit’s depth buffer.

var triangleFillMode: SimpleMaterial.TriangleFillMode

The object that controls how RealityKit draws triangles.

var writesDepth: Bool

A boolean value that determines whether this material writes its depth into RealityKit’s depth buffer.

### Type Aliases

typealias FaceCulling

An alias for the cull mode object that’s appropriate for this material class.

typealias TriangleFillMode

### Default Implementations

Material Implementations

## Relationships

### Conforms To

- Material

## See Also

### Simple materials

typealias BaseColor

The type used to represent base color.

typealias Texture

The type used to represent textures.

typealias Parameters

The parameter type that custom materials uses for properties the framework passes to shader functions.

typealias FaceCulling

An alias for the cull mode object that’s appropriate for this material class.

typealias TriangleFillMode

