

- SceneKit
- SCNGeometryElement
-  primitiveRange 

Instance Property

# primitiveRange

The range of primitives from the geometry element to render.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var primitiveRange: NSRange { get set }
```

## Discussion

The default value for this property is an NSRange whose location is NSNotFound and length is zero, indicating that, by default, SceneKit renders the entire set of primitives specified by a geometry element’s data buffer.

You can change a geometry without redefining it by choosing to render only a subset of the primitives specified by a geometry element. To do so, set this property to a subrange of primitive indexes.

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

var primitiveCount: Int

The number of primitives in the element.

