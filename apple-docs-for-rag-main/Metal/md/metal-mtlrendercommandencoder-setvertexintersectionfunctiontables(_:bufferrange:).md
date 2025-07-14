

- Metal
- MTLRenderCommandEncoder
-  setVertexIntersectionFunctionTables(\_:bufferRange:) 

Instance Method

# setVertexIntersectionFunctionTables(\_:bufferRange:)

Assigns multiple intersection function tables to a range of entries in the vertex shader argument table.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 16.0+visionOS

``` source
func setVertexIntersectionFunctionTables(
    _ functionTables: [(any MTLIntersectionFunctionTable)?],
    bufferRange: Range
)
```

## Parameters 

`functionTables`  

An array of MTLIntersectionFunctionTable instances the command assigns to entries in the vertex shader argument table for intersection function tables.

`bufferRange`  

A span of integers that represent the entries in the vertex shader argument table for intersection function tables. Each entry stores a record of the corresponding element in `functionTables`.

## Discussion

By default, the intersection function table at each index is `nil`.

Note

The Objective-C version of this method is setVertexIntersectionFunctionTables:withBufferRange:.

## See Also

### Assigning Intersection Function Tables

func setVertexIntersectionFunctionTable((any MTLIntersectionFunctionTable)?, bufferIndex: Int)

Assigns an intersection function table to an entry in the vertex shader argument table.

**Required**

