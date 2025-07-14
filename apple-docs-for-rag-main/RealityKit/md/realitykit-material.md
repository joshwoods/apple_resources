

- RealityKit
-  Material 

Protocol

# Material

A type that describes the material aspects of a mesh, like color and texture.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
protocol Material
```

## Mentioned in 

Applying realistic material and lighting effects to entities

Adding procedural assets to a scene

## Overview

In RealityKit, a *material* defines the surface properties of a 3D model. It specifies how RealityKit renders the entity, including its color and whether it’s shiny or reflective. A ModelEntity may have one material that defines the way RealityKit renders the entire entity, or it may have several that define the look of different parts of the model.

RealityKit provides several different material structures for different types of rendering, including PhysicallyBasedMaterial, which is a versatile material capable of simulating real-world objects in a highly realistic manner, and UnlitMaterial, which RealityKit draws with no lighting effects or shadows.

If you import a model from a USDZ file, RealityKit automatically creates one or more PhysicallyBasedMaterial instances from the material properties contained in the file.

## Topics

### Identifying a material

var name: String?

Name exported with USDz or Reality File asset

### Type Aliases

typealias Color

An alias for the color type that’s appropriate for the current platform.

typealias Parameters

The parameter type that custom materials uses for properties the framework passes to shader functions.

## Relationships

### Conforming Types

- CustomMaterial
- OcclusionMaterial
- PhysicallyBasedMaterial
- PortalMaterial
- ShaderGraphMaterial
- SimpleMaterial
- UnlitMaterial
- VideoMaterial

## See Also

### Material types

typealias Color

An alias for the color type that’s appropriate for the current platform.

typealias Parameters

The parameter type that custom materials uses for properties the framework passes to shader functions.

struct MaterialParameterTypes

A set of types that material parameters can use.

struct MaterialParameters

enum MaterialColorParameter

The color parameter applied to a material.

enum MaterialScalarParameter

The scalar parameter applied to a material.

