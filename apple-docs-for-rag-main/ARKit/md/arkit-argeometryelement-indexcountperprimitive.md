

- ARKit
- ARGeometryElement
-  indexCountPerPrimitive 

Instance Property

# indexCountPerPrimitive

The number of indices for each primitive.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+

``` source
var indexCountPerPrimitive: Int { get }
```

## Discussion

The value of this property relates to the primitiveType. For ARGeometryPrimitiveType.triangle, the value is 3. For more information, see ARGeometryPrimitiveType.

## See Also

### Getting Index Information

var bytesPerIndex: Int

The number of bytes for each index.

var count: Int

The number of primitives in the buffer.

var primitiveType: ARGeometryPrimitiveType

The geometry’s type of data (triangle, or line).

enum ARGeometryPrimitiveType

The kind of connection between vertices.

