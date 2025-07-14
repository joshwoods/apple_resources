

- Model I/O
- MDLMesh
-  vertexAttributeData(forAttributeNamed:) 

Instance Method

# vertexAttributeData(forAttributeNamed:)

Returns the vertex data for the specified attribute.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func vertexAttributeData(forAttributeNamed name: String) -> MDLVertexAttributeData?
```

## Parameters 

`name`  

The attribute name for which to retrieve data. See Vertex Attributes for standard attribute names.

## Return Value

The vertex data for the specified attribute, or `nil` if the mesh does not contain vertex data for the specified attribute.

## Discussion

Calling this data is equivalent to using the mesh’s vertexDescriptor object to find the index of the MDLMeshBuffer object corresponding to the specified vertex attribute in the mesh’s vertexBuffers array, then using the vertex buffer’s map() method to gain read-only access to the vertex buffer’s data.

Important

The buffer’s storage remains mapped for as long as the returned MDLVertexAttributeData object exists, potentially restricting other uses of that storage. For example, if a buffer’s storage is shared with GPU memory, that buffer may be unavailable for use in rendering until the data object is deallocated.

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

func addUnwrappedTextureCoordinates(forAttributeNamed: String)

func vertexAttributeData(forAttributeNamed: String, as: MDLVertexFormat) -> MDLVertexAttributeData?

