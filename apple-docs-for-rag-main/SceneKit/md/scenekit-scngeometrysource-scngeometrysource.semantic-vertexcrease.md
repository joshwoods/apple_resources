

- SceneKit
- SCNGeometrySource
- SCNGeometrySource.Semantic
-  vertexCrease 

Type Property

# vertexCrease

The semantic for vertex crease data, used for subdividing surfaces.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
static let vertexCrease: SCNGeometrySource.Semantic
```

## Discussion

For a geometry source, this semantic identifies data containing crease data for each vertex in the geometry. SceneKit uses this information to determine the sharpness of corners and smoothness of surfaces when you change a geometry’s subdivisionLevel property.

For a custom shader program, you use this semantic to bind SceneKit’s vertex crease data to an input attribute of the shader.

Vertex crease data is an array of scalar floating-point values, where each value determines the smoothness or sharpness of the corresponding vertex: A value of `0.0` specifies a completely smoothed corner, and a value of `10.0` or greater specifies an infinitely sharp point.

## See Also

### Surface Subdivision Semantics

static let edgeCrease: SCNGeometrySource.Semantic

The semantic for edge crease data, used for subdividing surfaces.

