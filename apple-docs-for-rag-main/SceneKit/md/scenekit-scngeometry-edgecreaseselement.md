

- SceneKit
- SCNGeometry
-  edgeCreasesElement 

Instance Property

# edgeCreasesElement

The geometry element identifying which edges of the geometry’s surface should remain sharp after subdivision.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var edgeCreasesElement: SCNGeometryElement? { get set }
```

## Discussion

This geometry element’s primitiveType value must be SCNGeometryPrimitiveType.line. The geometry element’s data is an array of vertex indices, each pair of which defines a line segment identifying an edge to be treated as a crease during subdivision. Use the edgeCreasesSource property to specify the smoothness or sharpness of each crease.

## See Also

### Smoothing and Subdividing Geometry

var subdivisionLevel: Int

The number of subdivisions SceneKit uses to smooth the geometry’s surface at render time.

var edgeCreasesSource: SCNGeometrySource?

The geometry source specifying the smoothness or sharpness of edges after surface subdivision.

var wantsAdaptiveSubdivision: Bool

