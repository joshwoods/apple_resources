

- Metal
- MTLRenderCommandEncoder
-  setThreadgroupMemoryLength(\_:offset:index:) 

Instance Method

# setThreadgroupMemoryLength(\_:offset:index:)

Configures the size of a threadgroup memory buffer for an entry in the fragment or tile shader argument table.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.5+visionOS 1.0+

``` source
func setThreadgroupMemoryLength(
    _ length: Int,
    offset: Int,
    index: Int
)
```

**Required**

## Parameters 

`length`  

The threadgroup memory length, in bytes.

`offset`  

An integer that represents the location, in bytes, from the start of the buffer at `index` where the threadgroup memory begins.

`index`  

An integer that represents an entry in the buffer argument table.

## Discussion

You can only change the threadgroup memory’s size between tile dispatches (see dispatchThreadsPerTile(_:)).

Important

Exceeding the threadgroup memory allocation for the render pass can trigger a debug error.

## See Also

### Configuring Persistent Threadgroup Memory

func setObjectThreadgroupMemoryLength(Int, index: Int)

Configures the size of a threadgroup memory buffer for an entry in the object argument table.

**Required**

