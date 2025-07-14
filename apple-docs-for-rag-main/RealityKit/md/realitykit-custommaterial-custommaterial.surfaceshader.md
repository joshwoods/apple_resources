

- RealityKit
- CustomMaterial
-  CustomMaterial.SurfaceShader 

Structure

# CustomMaterial.SurfaceShader

The custom material’s surface shader function.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
struct SurfaceShader
```

## Overview

Custom materials work together with a surface shader function to render entities. The CustomMaterial properties related to rendering, such as baseColor and normal, are available in the surface shader function, but RealityKit doesn’t use them directly.

Instead, the material’s surface shader function allows you to calculate or specify all the material parameters that RealityKit uses to render your entity, such as baseColor, normal, and roughness. RealityKit’s fragment shader calls your surface shader function once for each pixel it renders.

Here’s a simple example of a surface shader that sets the entity’s base color:

```
#include 
#include 

// Specify the current default namespace as metal so that it's not
// necessary to prefix Metal Standard Library symbols.
using namespace metal;

[[visible]] void mySurfaceShader(realitykit::surface_parameters params)
{
    // Set the base color
    params.surface().set_base_color(half3(1.0, 0.5, 0.5));
}
```

For more information on creating custom materials and writing shader functions, see Modifying RealityKit rendering using custom materials.

## Topics

### Creating surface shader objects

init(named: String, in: any MTLLibrary)

Creates a surface shader object from a named function in a Metal library.

### Accessing surface shader properties

var name: String

The name of the surface shader function.

var library: any MTLLibrary

The Metal library that contains this surface shader function.

### Initializers

init(named: String, in: any MTLLibrary, constantValues: MTLFunctionConstantValues)

Creates a surface shader with the specified function constant values.

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

struct GeometryModifier

The custom material’s optional shader function that can manipulate an entity’s vertex data.

protocol MaterialFunction

The abstract superclass for objects representing compute functions for RealityKit custom materials .

class Program

An object that represents the backing shader compilation required for custom materials.

struct Descriptor

An object that specifies all parameters necessary to initialize `CustomMaterial` programs

enum CustomShaderStage

