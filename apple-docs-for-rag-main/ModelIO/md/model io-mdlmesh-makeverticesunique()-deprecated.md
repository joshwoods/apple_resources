

- Model I/O
- MDLMesh
-  makeVerticesUnique() Deprecated

Instance Method

# makeVerticesUnique()

Modifies the mesh’s vertex buffers so that no vertices are shared by multiple faces.

iOS 9.0–11.0DeprecatediPadOS 9.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.11–10.13DeprecatedtvOS 9.0–11.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func makeVerticesUnique()
```

## Discussion

If the same entry in the mesh’s vertex buffer is used in multiple faces (according to the index buffers of the mesh’s submeshes), this method duplicates that vertex data and modifies the vertex and index buffers accordingly. If such operations require a larger vertex or index buffer, this method uses the allocator property of the buffer in question to allocate new storage.

## See Also

### Generating Geometry Data

func addNormals(withAttributeNamed: String?, creaseThreshold: Float)

Generates surface normal data for the mesh based on its vertex position data.

func addTangentBasis(forTextureCoordinateAttributeNamed: String, tangentAttributeNamed: String, bitangentAttributeNamed: String?)

Generates surface tangent and bitangent data for the mesh based on its vertex position and texture coordinate data.

func addTangentBasis(forTextureCoordinateAttributeNamed: String, normalAttributeNamed: String, tangentAttributeNamed: String)

Generates surface tangent data for the mesh based on its vertex position, surface normal, and texture coordinate data.

