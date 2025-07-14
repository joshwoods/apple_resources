

- SceneKit
- SCNGeometry
-  edgeCreasesSource 

Instance Property

# edgeCreasesSource

The geometry source specifying the smoothness or sharpness of edges after surface subdivision.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var edgeCreasesSource: SCNGeometrySource? { get set }
```

## Discussion

This geometry source’s semantic value must be edgeCrease. Its data is an array of scalar values (that is, the source’s componentsPerVector value is `1`). The value at an index in the geometry source determines the smoothness or sharpness of the edge identified by the primitive at the corresponding index in the edgeCreasesElement geometry element: a value of `0.0` specifies a completely smoothed edge, and a value of `10.0` or greater specifies an infinitely sharp edge.

## See Also

### Smoothing and Subdividing Geometry

var subdivisionLevel: Int

The number of subdivisions SceneKit uses to smooth the geometry’s surface at render time.

var edgeCreasesElement: SCNGeometryElement?

The geometry element identifying which edges of the geometry’s surface should remain sharp after subdivision.

var wantsAdaptiveSubdivision: Bool

