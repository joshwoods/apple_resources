

- Metal
- MTLComputeCommandEncoder
-  setVisibleFunctionTables(\_:bufferRange:) 

Instance Method

# setVisibleFunctionTables(\_:bufferRange:)

Binds multiple visible function tables to the buffer argument table, allowing you to call their functions on the GPU.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 16.0+visionOS

``` source
func setVisibleFunctionTables(
    _ visibleFunctionTables: [(any MTLVisibleFunctionTable)?],
    bufferRange: Range
)
```

## Parameters 

`visibleFunctionTables`  

An array of MTLVisibleFunctionTable instances to bind.

`bufferRange`  

The buffer argument table indices to bind each of the `visibleFunctionTables` to, in the order they appear.

## Discussion

Warning

This method requires that the number of instances in `visibleFunctionTables` be the same as the length of `bufferRange`.

## See Also

### Encoding Function Tables

func setVisibleFunctionTable((any MTLVisibleFunctionTable)?, bufferIndex: Int)

Binds a visible function table to the buffer argument table, allowing you to call its functions on the GPU.

**Required**

func setIntersectionFunctionTables([(any MTLIntersectionFunctionTable)?], bufferRange: Range&lt;Int>)

Binds multiple intersection function tables to the buffer argument table, allowing you to call their functions on the GPU.

