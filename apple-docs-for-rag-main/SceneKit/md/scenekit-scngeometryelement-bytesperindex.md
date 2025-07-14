

- SceneKit
- SCNGeometryElement
-  bytesPerIndex 

Instance Property

# bytesPerIndex

The number of bytes that represent each index value in the element’s data.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var bytesPerIndex: Int { get }
```

## Discussion

An element’s data property holds an array of index values identifying vertices in a geometry source. SceneKit interprets the data as an array of unsigned integers, whose size is specified by the bytesPerIndex property.

## See Also

### Working with Indexes

var data: Data

The data describing the geometry element.

var primitiveType: SCNGeometryPrimitiveType

The drawing primitive that connects vertices when rendering the geometry element.

enum SCNGeometryPrimitiveType

The drawing primitive that connects vertices when rendering a geometry element, used by the primitiveType property to specify how SceneKit interprets the geometry element’s data.

var primitiveCount: Int

The number of primitives in the element.

var primitiveRange: NSRange

The range of primitives from the geometry element to render.

