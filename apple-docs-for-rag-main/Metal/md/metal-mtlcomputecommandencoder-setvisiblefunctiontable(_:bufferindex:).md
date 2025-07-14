

- Metal
- MTLComputeCommandEncoder
-  setVisibleFunctionTable(\_:bufferIndex:) 

Instance Method

# setVisibleFunctionTable(\_:bufferIndex:)

Binds a visible function table to the buffer argument table, allowing you to call its functions on the GPU.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
func setVisibleFunctionTable(
    _ visibleFunctionTable: (any MTLVisibleFunctionTable)?,
    bufferIndex: Int
)
```

**Required**

## Parameters 

`visibleFunctionTable`  

The MTLVisibleFunctionTable to bind.

`bufferIndex`  

The index the function table binds to in the buffer argument table.

## See Also

### Encoding Function Tables

func setVisibleFunctionTables([(any MTLVisibleFunctionTable)?], bufferRange: Range&lt;Int>)

Binds multiple visible function tables to the buffer argument table, allowing you to call their functions on the GPU.

func setIntersectionFunctionTables([(any MTLIntersectionFunctionTable)?], bufferRange: Range&lt;Int>)

Binds multiple intersection function tables to the buffer argument table, allowing you to call their functions on the GPU.

