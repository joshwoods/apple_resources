

- RealityKit
-  MaterialColorParameter 

Enumeration

# MaterialColorParameter

The color parameter applied to a material.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
enum MaterialColorParameter
```

## Topics

### Selecting color parameters

case color(NSColor)

A color value in macOS.

case texture(TextureResource)

A texture resource.

### Comparing material color parameters

static func == (MaterialColorParameter, MaterialColorParameter) -> Bool

Indicates whether two color parameters are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

func hash(into: inout Hasher)

Hashes the essential components of the color parameter by feeding them into the given hash function.

var hashValue: Int

The hash value.

### Enumeration Cases

case color(UIColor)

A color value in macOS.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
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

enum MaterialScalarParameter

The scalar parameter applied to a material.

