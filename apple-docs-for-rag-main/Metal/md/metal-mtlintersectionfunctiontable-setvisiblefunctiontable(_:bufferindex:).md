

- Metal
- MTLIntersectionFunctionTable
-  setVisibleFunctionTable(\_:bufferIndex:) 

Instance Method

# setVisibleFunctionTable(\_:bufferIndex:)

Sets a visible function table for the intersection functions.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
func setVisibleFunctionTable(
    _ functionTable: (any MTLVisibleFunctionTable)?,
    bufferIndex: Int
)
```

**Required**

## Parameters 

`functionTable`  

A visible function table.

`bufferIndex`  

An index in the function table’s buffer argument table.

## See Also

### Specifying Arguments for Intersection Functions

func setBuffer((any MTLBuffer)?, offset: Int, index: Int)

Sets a buffer for the intersection functions.

**Required**

func setBuffers([(any MTLBuffer)?], offsets: [Int], range: Range&lt;Int>)

Sets a range of buffers for the intersection functions.

func setVisibleFunctionTables([(any MTLVisibleFunctionTable)?], bufferRange: Range&lt;Int>)

Sets a range of visible function tables for the intersection functions.

