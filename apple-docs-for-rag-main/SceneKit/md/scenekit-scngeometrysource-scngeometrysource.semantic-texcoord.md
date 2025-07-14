

- SceneKit
- SCNGeometrySource
- SCNGeometrySource.Semantic
-  texcoord 

Type Property

# texcoord

The semantic for texture coordinate data.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static let texcoord: SCNGeometrySource.Semantic
```

## Discussion

For a geometry source, this semantic identifies data containing texture mapping coordinates for each vertex in the geometry. Unlike other semantics, a geometry may contain multiple sources for texture coordinates—each corresponds to a separate mappingChannel number that you can use when associating textured materials.

For a custom shader program, you use this semantic to bind SceneKit’s texture coordinate data to one or more input attributes of the shader.

Texture coordinate data is typically an array of two-component vectors.

## See Also

### Basic Geometry Semantics

static let vertex: SCNGeometrySource.Semantic

The semantic for vertex position data.

static let normal: SCNGeometrySource.Semantic

The semantic for surface normal data.

