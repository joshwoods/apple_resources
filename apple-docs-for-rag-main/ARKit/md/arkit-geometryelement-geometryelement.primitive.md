

- ARKit
- GeometryElement
-  GeometryElement.Primitive 

Enumeration

# GeometryElement.Primitive

The kind of primitive, lines or triangles, that a geometry element contains.

visionOS 1.0+

``` source
enum Primitive
```

## Topics

### Primitive shapes

case line

Two vertices that connect to form a line.

case triangle

Three vertices that connect to form a triangle.

### Inspecting geometry primitives

var indexCount: Int

The number of indices for the `Primitive`.

### Instance Properties

var description: String

A textual representation of GeometryElement.Primitive

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Equatable
- Hashable
- Sendable

## See Also

### Rendering geometry elements

var buffer: any MTLBuffer

A Metal buffer that contains index data that defines the geometry of an object.

var primitive: GeometryElement.Primitive

Get the type of the geometry element.

var count: Int

The number of primitives in the Metal buffer for a geometry element.

var bytesPerIndex: Int

The number of bytes that represent an index value.

var description: String

A textual representation of this geometry element.

