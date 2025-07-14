

- RealityKit
- CustomMaterial
- CustomMaterial.Program
-  CustomMaterial.Program.Descriptor 

Structure

# CustomMaterial.Program.Descriptor

An object that specifies all parameters necessary to initialize `CustomMaterial` programs

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+

``` source
struct Descriptor
```

## Topics

### Operators

static func == (CustomMaterial.Program.Descriptor, CustomMaterial.Program.Descriptor) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init()

### Instance Properties

var blendMode: MaterialParameterTypes.BlendMode?

Modes that describe how materials using the created `CustomMaterial.Program` will be blended with content behind them.

var hashValue: Int

The hash value.

var lightingModel: CustomMaterial.LightingModel

Modes that describe how materials using created `CustomMaterial.Program` will interact with light within the RealityKit scene.

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

enum CustomShaderStage

