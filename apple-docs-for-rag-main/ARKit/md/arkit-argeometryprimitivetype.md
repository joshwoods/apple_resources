

- ARKit
-  ARGeometryPrimitiveType 

Enumeration

# ARGeometryPrimitiveType

The kind of connection between vertices.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+

``` source
enum ARGeometryPrimitiveType
```

## Overview

When you enable sceneReconstruction on a world-tracking configuration, ARKit provies a wireframe mesh that models the shape of the real world using a collection of connected vertices. ARKit uses ARGeometryPrimitiveType to indicate how a particular property of that mesh is interpreted. For example, a mesh geometry’s faces property specifies that each face within the geometry is of type ARGeometryPrimitiveType.triangle.

## Topics

### Type of Connection

case line

A line segment in which a line connects two vertices.

case triangle

Three vertices that connect to form a triangle.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting Index Information

var bytesPerIndex: Int

The number of bytes for each index.

var count: Int

The number of primitives in the buffer.

var indexCountPerPrimitive: Int

The number of indices for each primitive.

var primitiveType: ARGeometryPrimitiveType

The geometry’s type of data (triangle, or line).

