

- SceneKit
- SCNGeometryElement
-  primitiveType 

Instance Property

# primitiveType

The drawing primitive that connects vertices when rendering the geometry element.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var primitiveType: SCNGeometryPrimitiveType { get }
```

## Discussion

For possible values, see SCNGeometryPrimitiveType.

## See Also

### Working with Indexes

var data: Data

The data describing the geometry element.

var bytesPerIndex: Int

The number of bytes that represent each index value in the element’s data.

enum SCNGeometryPrimitiveType

The drawing primitive that connects vertices when rendering a geometry element, used by the primitiveType property to specify how SceneKit interprets the geometry element’s data.

var primitiveCount: Int

The number of primitives in the element.

var primitiveRange: NSRange

The range of primitives from the geometry element to render.

