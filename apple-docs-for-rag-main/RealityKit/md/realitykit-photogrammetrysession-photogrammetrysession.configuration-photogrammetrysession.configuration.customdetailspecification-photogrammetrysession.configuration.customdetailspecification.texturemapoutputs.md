

- RealityKit
- PhotogrammetrySession
- PhotogrammetrySession.Configuration
- PhotogrammetrySession.Configuration.CustomDetailSpecification
-  PhotogrammetrySession.Configuration.CustomDetailSpecification.TextureMapOutputs 

Structure

# PhotogrammetrySession.Configuration.CustomDetailSpecification.TextureMapOutputs

Allows specification of the set of output texture maps to be included in the output model.

Mac Catalyst 17.0+macOS 14.0+

``` source
struct TextureMapOutputs
```

## Topics

### Initializers

init(rawValue: UInt)

Creates a new option set from the given raw value.

### Instance Properties

let rawValue: UInt

The corresponding value of the raw type.

### Type Aliases

typealias ArrayLiteralElement

The type of the elements of an array literal.

typealias Element

The element type of the option set.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Type Properties

static let all: PhotogrammetrySession.Configuration.CustomDetailSpecification.TextureMapOutputs

Option to include all maps.

static let ambientOcclusion: PhotogrammetrySession.Configuration.CustomDetailSpecification.TextureMapOutputs

The ambient occlusion (AO) map.

static let diffuseColor: PhotogrammetrySession.Configuration.CustomDetailSpecification.TextureMapOutputs

The primary base color texture map.

static let displacement: PhotogrammetrySession.Configuration.CustomDetailSpecification.TextureMapOutputs

The surface displacement map.

static let normal: PhotogrammetrySession.Configuration.CustomDetailSpecification.TextureMapOutputs

The normal map.

static let roughness: PhotogrammetrySession.Configuration.CustomDetailSpecification.TextureMapOutputs

The surface roughness map.

### Default Implementations

Equatable Implementations

OptionSet Implementations

SetAlgebra Implementations

## Relationships

### Conforms To

- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- SetAlgebra

