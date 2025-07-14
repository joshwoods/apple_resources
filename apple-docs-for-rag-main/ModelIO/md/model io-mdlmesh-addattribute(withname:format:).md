

- Model I/O
- MDLMesh
-  addAttribute(withName:format:) 

Instance Method

# addAttribute(withName:format:)

Adds a vertex attribute to the mesh and creates a new, empty corresponding vertex buffer.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func addAttribute(
    withName name: String,
    format: MDLVertexFormat
)
```

## Parameters 

`name`  

A name for the new attribute. See Vertex Attributes for standard attribute names.

`format`  

The data format for the new attribute.

## Discussion

Calling this method updates the mesh’s vertexDescriptor object to reflect the new attribute, and then uses the same MDLMeshBufferAllocator object shared by the mesh’s existing vertex buffers to allocate new, empty storage for the new attribute’s vertex data. This method has no effect if the mesh already contains an attribute with the specified name; to overwrite or rearrange existing attribute data, use the vertexDescriptor property.

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

func addAttribute(withName: String, format: MDLVertexFormat, type: String, data: Data, stride: Int)

func addAttribute(withName: String, format: MDLVertexFormat, type: String, data: Data, stride: Int, time: TimeInterval)

func removeAttributeNamed(String)

func replaceAttributeNamed(String, with: MDLVertexAttributeData)

func updateAttributeNamed(String, with: MDLVertexAttributeData)

func addUnwrappedTextureCoordinates(forAttributeNamed: String)

func vertexAttributeData(forAttributeNamed: String) -> MDLVertexAttributeData?

Returns the vertex data for the specified attribute.

func vertexAttributeData(forAttributeNamed: String, as: MDLVertexFormat) -> MDLVertexAttributeData?

