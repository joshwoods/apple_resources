

- SceneKit
-  SCNGeometryPrimitiveType 

Enumeration

# SCNGeometryPrimitiveType

The drawing primitive that connects vertices when rendering a geometry element, used by the primitiveType property to specify how SceneKit interprets the geometry element’s data.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum SCNGeometryPrimitiveType
```

## Topics

### Constants

case triangles

The geometry element’s data is a sequence of triangles, with each triangle described by three new vertices.

case triangleStrip

The geometry element’s data is a sequence of triangles, with each triangle described by one new vertex and two vertices from the previous triangle.

case line

The geometry element’s data is a sequence of line segments, with each line segment described by two new vertices.

case point

The geometry element’s data is a sequence of unconnected points.

### Enumeration Cases

case polygon

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

### Working with Indexes

var data: Data

The data describing the geometry element.

var bytesPerIndex: Int

The number of bytes that represent each index value in the element’s data.

var primitiveType: SCNGeometryPrimitiveType

The drawing primitive that connects vertices when rendering the geometry element.

var primitiveCount: Int

The number of primitives in the element.

var primitiveRange: NSRange

The range of primitives from the geometry element to render.

