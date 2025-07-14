

- ARKit
-  ARGeometryElement 

Class

# ARGeometryElement

A container for index data, such as vertex indices of a face.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+

``` source
class ARGeometryElement
```

## Overview

ARMeshGeometry uses geometry-elements to store face data (see faces). Each face is defined by the primitive type, for example, ARGeometryPrimitiveType.triangle.

To demonstrate, an ARMeshGeometry instance with two triangle-type faces results in the following configuration:

- `faces` count `= 2`

- `faces` indexCountPerPrimitive `= 3` (because primitiveType is ARGeometryPrimitiveType.triangle)

- `faces` bytesPerIndex `= 4` (because vertex indices are the type UInt32)

- The buffer’s total size in bytes `=` count `*` indexCountPerPrimitive `*` bytesPerIndex (which in this case, is `2 * 3 * 4 = 24` bytes)

## Topics

### Accessing Index Data

subscript(Int) -> [Int32]

Provides an array of vertex indices that respresents the geometric primitive at the subscripted index.

var buffer: any MTLBuffer

A Metal buffer containing primitive data.

### Getting Index Information

var bytesPerIndex: Int

The number of bytes for each index.

var count: Int

The number of primitives in the buffer.

var indexCountPerPrimitive: Int

The number of indices for each primitive.

var primitiveType: ARGeometryPrimitiveType

The geometry’s type of data (triangle, or line).

enum ARGeometryPrimitiveType

The kind of connection between vertices.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Getting Geometry Information

var classification: ARGeometrySource?

Classification for each face in the mesh.

enum ARMeshClassification

Enumeration of different classes of real-world objects that ARKit can identify.

var faces: ARGeometryElement

An object that contains a buffer of vertex indices of the geometry’s faces.

var normals: ARGeometrySource

Rays that define which direction is outside for each face.

