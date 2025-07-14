

- RealityKit
- MeshBuffers
-  MeshBuffers.ElementType 

Enumeration

# MeshBuffers.ElementType

The data type for each element of the buffer.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
enum ElementType
```

## Topics

### Operators

static func == (MeshBuffers.ElementType, MeshBuffers.ElementType) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case double

case float

case int16

case int32

case int8

case jointInfluence

case simd2Float

case simd3Float

case simd4Float

case uInt16

case uInt32

case uInt8

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

- Copyable
- Equatable
- Hashable

