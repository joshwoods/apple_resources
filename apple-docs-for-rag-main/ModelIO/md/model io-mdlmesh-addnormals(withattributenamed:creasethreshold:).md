

- Model I/O
- MDLMesh
-  addNormals(withAttributeNamed:creaseThreshold:) 

Instance Method

# addNormals(withAttributeNamed:creaseThreshold:)

Generates surface normal data for the mesh based on its vertex position data.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func addNormals(
    withAttributeNamed attributeName: String?,
    creaseThreshold: Float
)
```

## Parameters 

`attributeName`  

The name of the vertex attribute for storing surface normal data. If `nil`, this method writes data into the MDLVertexAttributeNormal attribute by default.

`creaseThreshold`  

A value between `0.0` and `1.0` that determines the smoothness of normal generation between adjacent faces. Lower values interpolate sharper angles between faces into smooth surfaces, and higher values smooth only between faces that are nearly parallel. A value of `1.0` prevents smoothing, resulting in a faceted appearance.

## Discussion

Model I/O calculates surface normal vectors based on vertex positions using the common definition: The surface normal to a triangle is the normalized cross product of two sides of the triangle. For this method to calculate surface normals, the mesh must contain vertex data for the MDLVertexAttributePosition attribute. Calling this method on a mesh that does not contain vertex position data raises an exception.

The `creaseThreshold` parameter controls smoothing between adjacent faces. If two faces share an edge and are nearly parallel — that is, the dot product of their normal vectors is greater than the `creaseThreshold` value, this method generates a normal vector that interpolates between the two faces’ normal vectors. When shading with interpolated normal vectors, the two faces appear to be part of a smooth curve instead of two flat facets.

This method saves calculated normal data in the vertex attribute named in the `attributeName` parameter (by default, the MDLVertexAttributeNormal attribute). If the mesh already contains that attribute, this method overwrites the contents of the corresponding vertex buffer. If the mesh does not contain that attribute, this method creates a new attribute and updates the mesh’s vertexDescriptor object accordingly.

## See Also

### Generating Geometry Data

func addTangentBasis(forTextureCoordinateAttributeNamed: String, tangentAttributeNamed: String, bitangentAttributeNamed: String?)

Generates surface tangent and bitangent data for the mesh based on its vertex position and texture coordinate data.

func addTangentBasis(forTextureCoordinateAttributeNamed: String, normalAttributeNamed: String, tangentAttributeNamed: String)

Generates surface tangent data for the mesh based on its vertex position, surface normal, and texture coordinate data.

func makeVerticesUnique()

Modifies the mesh’s vertex buffers so that no vertices are shared by multiple faces.

Deprecated

