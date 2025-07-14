

- SceneKit
- SCNGeometry
-  subdivisionLevel 

Instance Property

# subdivisionLevel

The number of subdivisions SceneKit uses to smooth the geometry’s surface at render time.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var subdivisionLevel: Int { get set }
```

## Discussion

*Surface subdivision* is a technique for using low-detail geometry to generate a smooth surface for rendering. When you increase the subdivisionLevel value of a geometry, SceneKit automatically splits each face in the rendered surface, creating a more detailed, smoother geometry, as shown in . SceneKit performs this subdivision process at render time, preserving the original geometry data.

Subdividing a surface rounds away any sharp edges and corners in the geometry; however, such details may be important to a model’s design. To preserve edges, use the edgeCreasesElement property to identify edges and the edgeCreasesSource property to specify how smooth or sharp they should appear after subdivision. To preserve corners, include a geometry source whose semantic value is vertexCrease when creating the geometry.

The default subdivision level is zero, specifying no subdivision—SceneKit renders the geometry exactly as its vertex data specifies.

## See Also

### Smoothing and Subdividing Geometry

var edgeCreasesElement: SCNGeometryElement?

The geometry element identifying which edges of the geometry’s surface should remain sharp after subdivision.

var edgeCreasesSource: SCNGeometrySource?

The geometry source specifying the smoothness or sharpness of edges after surface subdivision.

var wantsAdaptiveSubdivision: Bool

