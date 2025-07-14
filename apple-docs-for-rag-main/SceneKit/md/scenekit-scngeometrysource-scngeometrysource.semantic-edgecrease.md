

- SceneKit
- SCNGeometrySource
- SCNGeometrySource.Semantic
-  edgeCrease 

Type Property

# edgeCrease

The semantic for edge crease data, used for subdividing surfaces.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
static let edgeCrease: SCNGeometrySource.Semantic
```

## Discussion

For a geometry source, this semantic identifies data containing crease data for each vertex in the geometry. SceneKit uses this information to determine the sharpness of edges and smoothness of surfaces when you change a geometry’s subdivisionLevel property.

For a custom shader program, you use this semantic to bind SceneKit’s edge crease data to an input attribute of the shader.

Edge crease data is an array of scalar floating-point values, where each value determines the smoothness or sharpness of the edge identified by the primitive at the corresponding index in the geometry’s SceneKit Constants geometry element: A value of `0.0` specifies a completely smoothed edge, and a value of `10.0` or greater specifies an infinitely sharp edge.

## See Also

### Surface Subdivision Semantics

static let vertexCrease: SCNGeometrySource.Semantic

The semantic for vertex crease data, used for subdividing surfaces.

