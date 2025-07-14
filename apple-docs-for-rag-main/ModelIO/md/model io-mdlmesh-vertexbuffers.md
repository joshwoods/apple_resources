

- Model I/O
- MDLMesh
-  vertexBuffers 

Instance Property

# vertexBuffers

The array of buffers that provide vertex data for the mesh.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var vertexBuffers: [any MDLMeshBuffer] { get set }
```

## Discussion

A mesh contains vertex data organized in one of two designs: as a *structure of arrays* or as an *array of structures*. In a structure of arrays, the mesh contains multiple vertex buffers, each of which provides data for a different vertex attribute, and a single vertex is the union of data from the same index in each of the separate buffers. In an array of structures, the mesh contains a single vertex buffer, and each index in the vertex buffer contains data for all vertex attributes. Use the vertexDescriptor property to determine the structure of the mesh’s vertex data.

## See Also

### Working with Vertex Data

var boundingBox: MDLAxisAlignedBoundingBox

The minimum region entirely enclosing the mesh’s vertex positions, expressed in the model coordinate system of the mesh.

var submeshes: NSMutableArray?

The array of submeshes to be used in rendering the mesh.

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

func addUnwrappedTextureCoordinates(forAttributeNamed: String)

func vertexAttributeData(forAttributeNamed: String) -> MDLVertexAttributeData?

Returns the vertex data for the specified attribute.

func vertexAttributeData(forAttributeNamed: String, as: MDLVertexFormat) -> MDLVertexAttributeData?

