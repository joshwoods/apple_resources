

- Model I/O
- MDLMesh
-  boundingBox 

Instance Property

# boundingBox

The minimum region entirely enclosing the mesh’s vertex positions, expressed in the model coordinate system of the mesh.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var boundingBox: MDLAxisAlignedBoundingBox { get }
```

## Discussion

This property’s value is valid only if the mesh contains vertex data for the MDLVertexAttributePosition attribute. If the mesh does not contain position information, this property’s value is a bounding box whose `maxBounds` coordinate is greater than its `minBounds` coordinate.

Reading this property for the first time processes the mesh’s vertex data to calculate and cache a bounding box. Reading this property thereafter returns the cached value.

## See Also

### Working with Vertex Data

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

func vertexAttributeData(forAttributeNamed: String) -> MDLVertexAttributeData?

Returns the vertex data for the specified attribute.

func vertexAttributeData(forAttributeNamed: String, as: MDLVertexFormat) -> MDLVertexAttributeData?

