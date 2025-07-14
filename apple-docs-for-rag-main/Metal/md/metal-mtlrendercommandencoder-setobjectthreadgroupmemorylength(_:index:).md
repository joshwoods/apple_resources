

- Metal
- MTLRenderCommandEncoder
-  setObjectThreadgroupMemoryLength(\_:index:) 

Instance Method

# setObjectThreadgroupMemoryLength(\_:index:)

Configures the size of a threadgroup memory buffer for an entry in the object argument table.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func setObjectThreadgroupMemoryLength(
    _ length: Int,
    index: Int
)
```

**Required**

## Parameters 

`length`  

The threadgroup memory length, in bytes.

`index`  

An integer that represents an entry in the object argument table.

## See Also

### Configuring Persistent Threadgroup Memory

func setThreadgroupMemoryLength(Int, offset: Int, index: Int)

Configures the size of a threadgroup memory buffer for an entry in the fragment or tile shader argument table.

**Required**

