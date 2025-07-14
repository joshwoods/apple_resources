

- RealityKit
- ShaderGraphMaterial
-  ShaderGraphMaterial.Error 

Enumeration

# ShaderGraphMaterial.Error

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
enum Error
```

## Topics

### Operators

static func == (ShaderGraphMaterial.Error, ShaderGraphMaterial.Error) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case incorrectTypeForParameterName

case parameterNameNotFound

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

Error Implementations

LocalizedError Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Error
- Hashable
- LocalizedError
- Sendable

