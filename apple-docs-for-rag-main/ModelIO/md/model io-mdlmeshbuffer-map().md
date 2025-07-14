

- Model I/O
- MDLMeshBuffer
-  map() 

Instance Method

# map()

Provides direct, read-only access to the buffer’s contents.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func map() -> MDLMeshBufferMap
```

**Required**

## Return Value

A data object mapped to the storage memory for the buffer.

## Discussion

The buffer’s storage remains mapped for as long as the returned MDLMeshBufferMap object exists, potentially restricting other uses of that storage. For example, if a buffer’s storage is shared with GPU memory, that buffer may be unavailable for use in rendering until the MDLMeshBufferMap object is deallocated.

## See Also

### Working with Data in a Buffer

func fill(Data, offset: Int)

Writes the specified data into the buffer.

**Required**

var length: Int

The data size of the buffer, in bytes.

**Required**

