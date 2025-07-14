

- Metal
- MTLIntersectionFunctionTable
-  setBuffers(\_:offsets:range:) 

Instance Method

# setBuffers(\_:offsets:range:)

Sets a range of buffers for the intersection functions.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 16.0+visionOS

``` source
func setBuffers(
    _ buffers: [(any MTLBuffer)?],
    offsets: [Int],
    range: Range
)
```

## Parameters 

`buffers`  

An array of buffers to insert into the table.

`offsets`  

An array of offsets to insert into the table.

`range`  

A range of indices in the function table’s buffer argument table.

## See Also

### Specifying Arguments for Intersection Functions

func setBuffer((any MTLBuffer)?, offset: Int, index: Int)

Sets a buffer for the intersection functions.

**Required**

func setVisibleFunctionTable((any MTLVisibleFunctionTable)?, bufferIndex: Int)

Sets a visible function table for the intersection functions.

**Required**

func setVisibleFunctionTables([(any MTLVisibleFunctionTable)?], bufferRange: Range&lt;Int>)

Sets a range of visible function tables for the intersection functions.

