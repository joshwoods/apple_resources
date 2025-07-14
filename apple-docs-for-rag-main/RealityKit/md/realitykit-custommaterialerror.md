

- RealityKit
-  CustomMaterialError 

Enumeration

# CustomMaterialError

Errors generated when loading custom material functions.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
enum CustomMaterialError
```

## Topics

### Operators

static func == (CustomMaterialError, CustomMaterialError) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case defaultSurfaceShaderForMaterialNotFound

case geometryModifierFunctionNotFound

case surfaceShaderFunctionNotFound

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

Error Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Error
- Hashable
- Sendable

