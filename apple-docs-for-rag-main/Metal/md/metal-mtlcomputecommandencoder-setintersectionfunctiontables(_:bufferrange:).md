

- Metal
- MTLComputeCommandEncoder
-  setIntersectionFunctionTables(\_:bufferRange:) 

Instance Method

# setIntersectionFunctionTables(\_:bufferRange:)

Binds multiple intersection function tables to the buffer argument table, allowing you to call their functions on the GPU.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 16.0+visionOS

``` source
func setIntersectionFunctionTables(
    _ intersectionFunctionTables: [(any MTLIntersectionFunctionTable)?],
    bufferRange: Range
)
```

## Parameters 

`intersectionFunctionTables`  

An array of MTLIntersectionFunctionTable instances to bind.

`bufferRange`  

The argument buffer table indices to bind each of the `intersectionFunctionTables` to, in the order they appear.

## Discussion

Warning

This method requires that the number of instances in `visibleFunctionTables` be the same as the length of `bufferRange`.

## See Also

### Encoding Function Tables

func setVisibleFunctionTable((any MTLVisibleFunctionTable)?, bufferIndex: Int)

Binds a visible function table to the buffer argument table, allowing you to call its functions on the GPU.

**Required**

func setVisibleFunctionTables([(any MTLVisibleFunctionTable)?], bufferRange: Range&lt;Int>)

Binds multiple visible function tables to the buffer argument table, allowing you to call their functions on the GPU.

