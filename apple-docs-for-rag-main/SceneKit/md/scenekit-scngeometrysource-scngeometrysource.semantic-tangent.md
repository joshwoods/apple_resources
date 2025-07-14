

- SceneKit
- SCNGeometrySource
- SCNGeometrySource.Semantic
-  tangent 

Type Property

# tangent

The semantic for surface tangent vector data.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
static let tangent: SCNGeometrySource.Semantic
```

## Discussion

For a geometry source, this semantic identifies data containing the surface tangent vector at each vertex in the geometry. SceneKit uses this information to compute advanced lighting effects on the surface.

For a custom shader program, you use this semantic to bind SceneKit’s vertex tangent data to an input attribute of the shader.

Vertex tangent data is typically an array of three- or four-component vectors.

## See Also

### Advanced Shading Semantics

static let color: SCNGeometrySource.Semantic

The semantic for per-vertex color data.

