

- Model I/O
- MDLMeshBufferData
-  init(type:data:) 

Initializer

# init(type:data:)

Initializes a buffer containing the specified data.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
init(
    type: MDLMeshBufferType,
    data: Data?
)
```

## Parameters 

`type`  

MDLMeshBufferType.vertex to create a buffer for a mesh’s vertex attribute data, or MDLMeshBufferType.index to create a buffer for a submesh’s index data.

`data`  

The initial data to copy into the buffer.

## Return Value

A new memory buffer for mesh data.

## See Also

### Creating a Buffer

init(type: MDLMeshBufferType, length: Int)

Initializes a buffer of the specified length.

