

- Metal
- MTLIntersectionFunctionTable
-  setBuffer(\_:offset:index:) 

Instance Method

# setBuffer(\_:offset:index:)

Sets a buffer for the intersection functions.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
func setBuffer(
    _ buffer: (any MTLBuffer)?,
    offset: Int,
    index: Int
)
```

**Required**

## Parameters 

`buffer`  

The MTLBuffer object to set in the argument table.

`offset`  

Where the data begins, in bytes, from the start of the buffer.

`index`  

An index in the function table’s buffer argument table.

## See Also

### Specifying Arguments for Intersection Functions

func setBuffers([(any MTLBuffer)?], offsets: [Int], range: Range&lt;Int>)

Sets a range of buffers for the intersection functions.

func setVisibleFunctionTable((any MTLVisibleFunctionTable)?, bufferIndex: Int)

Sets a visible function table for the intersection functions.

**Required**

func setVisibleFunctionTables([(any MTLVisibleFunctionTable)?], bufferRange: Range&lt;Int>)

Sets a range of visible function tables for the intersection functions.

