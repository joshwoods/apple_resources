

- SceneKit
- SCNGeometryElement
-  data 

Instance Property

# data

The data describing the geometry element.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var data: Data { get }
```

## Discussion

An element’s data is an array of index values identifying vertices in a geometry source. SceneKit interprets the data as an array of unsigned integers, whose size is specified by the bytesPerIndex property.

## See Also

### Working with Indexes

var bytesPerIndex: Int

The number of bytes that represent each index value in the element’s data.

var primitiveType: SCNGeometryPrimitiveType

The drawing primitive that connects vertices when rendering the geometry element.

enum SCNGeometryPrimitiveType

The drawing primitive that connects vertices when rendering a geometry element, used by the primitiveType property to specify how SceneKit interprets the geometry element’s data.

var primitiveCount: Int

The number of primitives in the element.

var primitiveRange: NSRange

The range of primitives from the geometry element to render.

