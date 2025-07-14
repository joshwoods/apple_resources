

- Model I/O
- MDLMeshBuffer
-  allocator 

Instance Property

# allocator

The allocator object that created the buffer.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var allocator: any MDLMeshBufferAllocator { get }
```

**Required**

## Discussion

Certain operations on the MDLMesh object that owns this buffer—for example, generating new vertex attributes with methods such as addNormals(withAttributeNamed:creaseThreshold:), or changing the format and layout of vertex data by assigning a new value to the vertexDescriptor property—may require reallocation of buffer memory. When you perform such operations, Model I/O uses the same allocator that was used to create the buffer.

## See Also

### Inspecting a Buffer

var zone: any MDLMeshBufferZone

The memory pool from which the buffer was created.

**Required**

var type: MDLMeshBufferType

The type of data contained in a buffer.

**Required**

