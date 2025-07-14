

- Model I/O
- MDLMeshBuffer
-  fill(\_:offset:) 

Instance Method

# fill(\_:offset:)

Writes the specified data into the buffer.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func fill(
    _ data: Data,
    offset: Int
)
```

**Required**

## Parameters 

`data`  

The data to be copied into the buffer.

`offset`  

The offset, in bytes, from the start of the buffer at which to write data.

## Discussion

If the length of the specified data (plus the `offset` parameter, if nonzero) is greater than the buffer’s length property, this method writes data only up to the end of the buffer.

## See Also

### Working with Data in a Buffer

func map() -> MDLMeshBufferMap

Provides direct, read-only access to the buffer’s contents.

**Required**

var length: Int

The data size of the buffer, in bytes.

**Required**

