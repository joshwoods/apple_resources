

- SceneKit
- SCNGeometryElement
-  primitiveCount 

Instance Property

# primitiveCount

The number of primitives in the element.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var primitiveCount: Int { get }
```

## See Also

### Working with Indexes

var data: Data

The data describing the geometry element.

var bytesPerIndex: Int

The number of bytes that represent each index value in the element’s data.

var primitiveType: SCNGeometryPrimitiveType

The drawing primitive that connects vertices when rendering the geometry element.

enum SCNGeometryPrimitiveType

The drawing primitive that connects vertices when rendering a geometry element, used by the primitiveType property to specify how SceneKit interprets the geometry element’s data.

var primitiveRange: NSRange

The range of primitives from the geometry element to render.

