

- SceneKit
- SCNGeometrySource
- SCNGeometrySource.Semantic
-  vertex 

Type Property

# vertex

The semantic for vertex position data.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static let vertex: SCNGeometrySource.Semantic
```

## Discussion

For a geometry source, this semantic identifies data containing the positions of each vertex in the geometry. If you create a custom geometry using the init(sources:elements:) method, you must provide a geometry source for this semantic.

For a custom shader program, you use this semantic to bind SceneKit’s vertex position data to an input attribute of the shader.

Vertex position data is typically an array of three- or four-component vectors.

## See Also

### Basic Geometry Semantics

static let normal: SCNGeometrySource.Semantic

The semantic for surface normal data.

static let texcoord: SCNGeometrySource.Semantic

The semantic for texture coordinate data.

