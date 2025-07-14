

- Model I/O
- MDLMesh
-  addUnwrappedTextureCoordinates(forAttributeNamed:) 

Instance Method

# addUnwrappedTextureCoordinates(forAttributeNamed:)

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func addUnwrappedTextureCoordinates(forAttributeNamed textureCoordinateAttributeName: String)
```

## See Also

### Working with Vertex Data

var boundingBox: MDLAxisAlignedBoundingBox

The minimum region entirely enclosing the mesh’s vertex positions, expressed in the model coordinate system of the mesh.

var submeshes: NSMutableArray?

The array of submeshes to be used in rendering the mesh.

var vertexBuffers: [any MDLMeshBuffer]

The array of buffers that provide vertex data for the mesh.

var vertexCount: Int

The number of vertices in the mesh.

var vertexDescriptor: MDLVertexDescriptor

A description of the format and layout of the mesh’s vertex buffers.

var allocator: any MDLMeshBufferAllocator

func addAttribute(withName: String, format: MDLVertexFormat)

Adds a vertex attribute to the mesh and creates a new, empty corresponding vertex buffer.

func addAttribute(withName: String, format: MDLVertexFormat, type: String, data: Data, stride: Int)

func addAttribute(withName: String, format: MDLVertexFormat, type: String, data: Data, stride: Int, time: TimeInterval)

func removeAttributeNamed(String)

func replaceAttributeNamed(String, with: MDLVertexAttributeData)

func updateAttributeNamed(String, with: MDLVertexAttributeData)

func vertexAttributeData(forAttributeNamed: String) -> MDLVertexAttributeData?

Returns the vertex data for the specified attribute.

func vertexAttributeData(forAttributeNamed: String, as: MDLVertexFormat) -> MDLVertexAttributeData?

