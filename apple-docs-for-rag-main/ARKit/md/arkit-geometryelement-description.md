

- ARKit
- GeometryElement
-  description 

Instance Property

# description

A textual representation of this geometry element.

visionOS 1.0+

``` source
var description: String { get }
```

## See Also

### Rendering geometry elements

var buffer: any MTLBuffer

A Metal buffer that contains index data that defines the geometry of an object.

var primitive: GeometryElement.Primitive

Get the type of the geometry element.

enum Primitive

The kind of primitive, lines or triangles, that a geometry element contains.

var count: Int

The number of primitives in the Metal buffer for a geometry element.

var bytesPerIndex: Int

The number of bytes that represent an index value.

