

- Model I/O
- MDLMeshBufferData
-  init(type:length:) 

Initializer

# init(type:length:)

Initializes a buffer of the specified length.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
init(
    type: MDLMeshBufferType,
    length: Int
)
```

## Parameters 

`type`  

MDLMeshBufferType.vertex to create a buffer for a mesh’s vertex attribute data, or MDLMeshBufferType.index to create a buffer for a submesh’s index data.

`length`  

The size, in bytes, of the buffer to create.

## Return Value

A new memory buffer for mesh data.

## Discussion

All bytes in the newly created buffer are zero.

## See Also

### Creating a Buffer

init(type: MDLMeshBufferType, data: Data?)

Initializes a buffer containing the specified data.

