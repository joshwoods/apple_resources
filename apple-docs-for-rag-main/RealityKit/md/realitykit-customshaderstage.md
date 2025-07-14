

- RealityKit
-  CustomShaderStage 

Enumeration

# CustomShaderStage

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+

``` source
enum CustomShaderStage
```

## Topics

### Operators

static func == (CustomShaderStage, CustomShaderStage) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case geometryModifier

case surfaceShader

### Instance Properties

var hashValue: Int

The hash value.

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

class Program

An object that represents the backing shader compilation required for custom materials.

struct Descriptor

An object that specifies all parameters necessary to initialize `CustomMaterial` programs

