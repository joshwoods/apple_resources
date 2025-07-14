

- RealityKit
- CustomMaterial
-  CustomMaterial.GeometryModifier 

Structure

# CustomMaterial.GeometryModifier

The custom material’s optional shader function that can manipulate an entity’s vertex data.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
struct GeometryModifier
```

## Overview

A geometry modifier is an optional Metal function that you can use with custom materials. Use a geometry modifier to change vertex data, such as vertex position, color, or texture coordinates. For example, offsetting a vertex’s position changes the size and shape of the entity for rendering only. If your custom material has a geometry modifier, RealityKit’s custom material vertex shader calls it once for each vertex in the entity. Changes that your geometry modifier makes are transient and don’t affect the vertex positions of the original ModelEntity.

Here’s a simple example of a geometry modifier that offsets the vertex positions along the z-axis based on the elapsed time:

```
#include 
#include 
using namespace metal;

[[visible]] void myGeometryModifier(realitykit::geometry_parameters
params) {
    float3 zOffset = float3(0.0, 0.0, params.uniforms().time() / 50.0);
    params.geometry().set_world_position_offset(zOffset);
}
```

For more information on creating custom materials and writing shader functions, see Modifying RealityKit rendering using custom materials.

## Topics

### Creating geometry modifier objects

init(named: String, in: any MTLLibrary)

Creates a geometry modifier object from a named function in a Metal library.

### Accessing geometry modifier properties

var name: String

The name of the geometry modifier function.

var library: any MTLLibrary

The Metal library that contains this surface shader function.

### Initializers

init(named: String, in: any MTLLibrary, constantValues: MTLFunctionConstantValues)

Creates a geometry modifier with the specified function constant values.

### Default Implementations

Equatable Implementations

Hashable Implementations

MaterialFunction Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- MaterialFunction
- Sendable

## See Also

### Shaders

struct ShaderGraphMaterial

typealias FaceCulling

An alias for the cull mode object that’s appropriate for this material class.

typealias TriangleFillMode

An alias for the triangle fill mode object that’s appropriate for this material class.

Modifying RealityKit rendering using custom materials

Write Metal shader functions to implement custom rendering effects.

struct CustomMaterial

A material that works with custom Metal shader functions.

struct SurfaceShader

The custom material’s surface shader function.

protocol MaterialFunction

The abstract superclass for objects representing compute functions for RealityKit custom materials .

class Program

An object that represents the backing shader compilation required for custom materials.

struct Descriptor

An object that specifies all parameters necessary to initialize `CustomMaterial` programs

enum CustomShaderStage

