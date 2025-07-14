

- RealityKit
- CustomMaterial
-  CustomMaterial.Program 

Class

# CustomMaterial.Program

An object that represents the backing shader compilation required for custom materials.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+

``` source
final class Program
```

## Overview

You can use this type to control when RealityKit compiles shaders, and to initialize `CustomMaterial` objects with more predicitable loading performance.

When initializing a `CustomMaterial` this way, a `Program` object is created first asynchronously, which is used to cache the material’s shader program so the `CustomMaterial` can be loaded immediately later.

For example:

```
// Initialize descriptor with desired properties
var descriptor = CustomMaterial.Descriptor()
descriptor.lightingModel = .unlit

// Create program object
let program = await CustomMaterial.Program(surfaceShader: surfaceShader,
                                           descriptor: descriptor)

// Create material (returns immediately)
let material = CustomMaterial(program: program)
```

## Topics

### Structures

struct Descriptor

An object that specifies all parameters necessary to initialize `CustomMaterial` programs

### Operators

static func == (CustomMaterial.Program, CustomMaterial.Program) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(surfaceShader: CustomMaterial.SurfaceShader, geometryModifier: CustomMaterial.GeometryModifier?, descriptor: CustomMaterial.Program.Descriptor) async throws

### Instance Properties

let descriptor: CustomMaterial.Program.Descriptor

let geometryModifier: CustomMaterial.GeometryModifier?

var hashValue: Int

The hash value.

let surfaceShader: CustomMaterial.SurfaceShader

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
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

struct GeometryModifier

The custom material’s optional shader function that can manipulate an entity’s vertex data.

protocol MaterialFunction

The abstract superclass for objects representing compute functions for RealityKit custom materials .

struct Descriptor

An object that specifies all parameters necessary to initialize `CustomMaterial` programs

enum CustomShaderStage

