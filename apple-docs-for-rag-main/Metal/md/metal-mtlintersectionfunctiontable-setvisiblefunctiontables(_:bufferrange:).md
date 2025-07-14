

- Metal
- MTLIntersectionFunctionTable
-  setVisibleFunctionTables(\_:bufferRange:) 

Instance Method

# setVisibleFunctionTables(\_:bufferRange:)

Sets a range of visible function tables for the intersection functions.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 16.0+visionOS

``` source
func setVisibleFunctionTables(
    _ functionTables: [(any MTLVisibleFunctionTable)?],
    bufferRange: Range
)
```

## Parameters 

`functionTables`  

The function tables to insert.

`bufferRange`  

A range of indices in the function table’s buffer argument table.

## See Also

### Specifying Arguments for Intersection Functions

func setBuffer((any MTLBuffer)?, offset: Int, index: Int)

Sets a buffer for the intersection functions.

**Required**

func setBuffers([(any MTLBuffer)?], offsets: [Int], range: Range&lt;Int>)

Sets a range of buffers for the intersection functions.

func setVisibleFunctionTable((any MTLVisibleFunctionTable)?, bufferIndex: Int)

Sets a visible function table for the intersection functions.

**Required**

