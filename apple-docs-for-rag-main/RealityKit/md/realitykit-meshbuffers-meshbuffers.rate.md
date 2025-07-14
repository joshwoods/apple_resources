

- RealityKit
- MeshBuffers
-  MeshBuffers.Rate 

Enumeration

# MeshBuffers.Rate

Defines how elements in the buffer map to features of the mesh.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
enum Rate
```

## Topics

### Operators

static func == (MeshBuffers.Rate, MeshBuffers.Rate) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case face

Buffer maps at the face rate.

case faceVarying

Buffer maps at the index rate.

case vertex

Buffer maps at the vertex rate.

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

