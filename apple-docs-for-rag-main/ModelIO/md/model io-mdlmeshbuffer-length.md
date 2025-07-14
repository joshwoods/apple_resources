

- Model I/O
- MDLMeshBuffer
-  length 

Instance Property

# length

The data size of the buffer, in bytes.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var length: Int { get }
```

**Required**

## See Also

### Working with Data in a Buffer

func fill(Data, offset: Int)

Writes the specified data into the buffer.

**Required**

func map() -> MDLMeshBufferMap

Provides direct, read-only access to the buffer’s contents.

**Required**

