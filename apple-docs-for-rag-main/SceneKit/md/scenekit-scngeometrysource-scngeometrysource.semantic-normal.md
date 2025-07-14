

- SceneKit
- SCNGeometrySource
- SCNGeometrySource.Semantic
-  normal 

Type Property

# normal

The semantic for surface normal data.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static let normal: SCNGeometrySource.Semantic
```

## Discussion

For a geometry source, this semantic identifies data containing the surface normal vector at each vertex in the geometry. SceneKit uses this information to compute lighting effects on the surface.

For a custom shader program, you use this semantic to bind SceneKit’s vertex normal data to an input attribute of the shader.

Vertex normal data is typically an array of three- or four-component vectors.

## See Also

### Basic Geometry Semantics

static let vertex: SCNGeometrySource.Semantic

The semantic for vertex position data.

static let texcoord: SCNGeometrySource.Semantic

The semantic for texture coordinate data.

