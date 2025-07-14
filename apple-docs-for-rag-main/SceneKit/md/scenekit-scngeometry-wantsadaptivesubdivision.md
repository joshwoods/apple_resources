

- SceneKit
- SCNGeometry
-  wantsAdaptiveSubdivision 

Instance Property

# wantsAdaptiveSubdivision

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var wantsAdaptiveSubdivision: Bool { get set }
```

## See Also

### Smoothing and Subdividing Geometry

var subdivisionLevel: Int

The number of subdivisions SceneKit uses to smooth the geometry’s surface at render time.

var edgeCreasesElement: SCNGeometryElement?

The geometry element identifying which edges of the geometry’s surface should remain sharp after subdivision.

var edgeCreasesSource: SCNGeometrySource?

The geometry source specifying the smoothness or sharpness of edges after surface subdivision.

