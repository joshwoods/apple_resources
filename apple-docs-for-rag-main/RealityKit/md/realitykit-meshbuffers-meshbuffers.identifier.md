

- RealityKit
- MeshBuffers
-  MeshBuffers.Identifier 

Structure

# MeshBuffers.Identifier

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
struct Identifier
```

## Topics

### Operators

static func == (MeshBuffers.Identifier, MeshBuffers.Identifier) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var description: String

A textual representation of this instance.

var hashValue: Int

The hash value.

let isBlendShape: Bool

let isCustom: Bool

let name: String

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Properties

static let bitangents: MeshBuffers.Identifier

static let jointInfluences: MeshBuffers.Identifier

static let normals: MeshBuffers.Identifier

static let positions: MeshBuffers.Identifier

static let tangents: MeshBuffers.Identifier

static let textureCoordinates: MeshBuffers.Identifier

static let triangleIndices: MeshBuffers.Identifier

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- CustomStringConvertible
- Equatable
- Hashable
- Sendable

