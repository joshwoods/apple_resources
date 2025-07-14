

- RealityKit
-  ShaderGraphMaterial 

Structure

# ShaderGraphMaterial

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
struct ShaderGraphMaterial
```

## Topics

### Initializers

init(materialXLabel: String, data: Data) async throws

Loads a ShaderGraphMaterial from MaterialX data.

init(named: String, from: URL) async throws

Loads a ShaderGraphMaterial from a url.

init(named: String, from: Data) async throws

Loads a ShaderGraphMaterial from a named material within a USD file.

init(named: String, from: String, in: Bundle?) async throws

Loads a ShaderGraphMaterial from a bundle.

### Instance Properties

var faceCulling: ShaderGraphMaterial.FaceCulling

A process in which the system specifies polygons to remove before rendering a mesh using this material.

var parameterNames: [String]

var readsDepth: Bool

A boolean value that determines whether this material performs the depth test by reading RealityKit’s depth buffer.

var triangleFillMode: ShaderGraphMaterial.TriangleFillMode

The object that controls how RealityKit draws triangles.

var writesDepth: Bool

A boolean value that determines whether this material writes its depth into RealityKit’s depth buffer.

### Instance Methods

func getParameter(handle: MaterialParameters.Handle) -> MaterialParameters.Value?

func getParameter(name: String) -> MaterialParameters.Value?

func setParameter(handle: MaterialParameters.Handle, value: MaterialParameters.Value) throws

func setParameter(name: String, value: MaterialParameters.Value) throws

### Type Aliases

typealias FaceCulling

An alias for the cull mode object that’s appropriate for this material class.

typealias TriangleFillMode

An alias for the triangle fill mode object that’s appropriate for this material class.

### Type Methods

static func parameterHandle(name: String) -> MaterialParameters.Handle

### Enumerations

enum Error

enum LoadError

### Default Implementations

Material Implementations

## Relationships

### Conforms To

- Material
- Sendable

## See Also

### Shaders

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

enum CustomShaderStage

