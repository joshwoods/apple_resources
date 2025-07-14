

- RealityKit
- MaterialParameterTypes
-  MaterialParameterTypes.TriangleFillMode 

Enumeration

# MaterialParameterTypes.TriangleFillMode

An object that defines how the system rasterizes triangles and triangle strips

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
enum TriangleFillMode
```

## Topics

### Operators

static func == (MaterialParameterTypes.TriangleFillMode, MaterialParameterTypes.TriangleFillMode) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case fill

Triangles and triangle strips are rasterized as filled triangles

case lines

Triangles and triangle strips are rasterized as lines

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

