

- RealityKit
-  MaterialScalarParameter 

Enumeration

# MaterialScalarParameter

The scalar parameter applied to a material.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
enum MaterialScalarParameter
```

## Topics

### Getting scalar parameters

case float(Float)

A scalar, single-precision value.

case texture(TextureResource)

A one-channel texture.

### Creating a scalar parameter

init(floatLiteral: Float)

Creates a scalar parameter from a floating-point literal.

init(integerLiteral: Int)

Creates a scalar parameter from an integer literal.

typealias FloatLiteralType

A type that represents a floating-point literal.

typealias IntegerLiteralType

A type that represents an integer literal.

### Comparing material scalar parameters

static func == (MaterialScalarParameter, MaterialScalarParameter) -> Bool

Indicates whether two scalar parameters are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

func hash(into: inout Hasher)

Hashes the essential components of the scalar parameter by feeding them into the given hash function.

var hashValue: Int

The hash value.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- ExpressibleByFloatLiteral
- ExpressibleByIntegerLiteral
- Hashable

## See Also

### Material types

protocol Material

A type that describes the material aspects of a mesh, like color and texture.

typealias Color

An alias for the color type that’s appropriate for the current platform.

typealias Parameters

The parameter type that custom materials uses for properties the framework passes to shader functions.

struct MaterialParameterTypes

A set of types that material parameters can use.

struct MaterialParameters

enum MaterialColorParameter

The color parameter applied to a material.

