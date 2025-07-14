

- Metal
- MTLRenderCommandEncoder
-  setVertexIntersectionFunctionTable(\_:bufferIndex:) 

Instance Method

# setVertexIntersectionFunctionTable(\_:bufferIndex:)

Assigns an intersection function table to an entry in the vertex shader argument table.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
func setVertexIntersectionFunctionTable(
    _ intersectionFunctionTable: (any MTLIntersectionFunctionTable)?,
    bufferIndex: Int
)
```

**Required**

## Parameters 

`intersectionFunctionTable`  

An MTLIntersectionFunctionTable instance the command assigns to an entry in the vertex shader argument table for intersection function tables.

`bufferIndex`  

An integer that represents the entry in the vertex shader argument table for intersection function tables that stores a record of `intersectionFunctionTable`.

## Discussion

By default, the intersection function table at each index is `nil`.

## See Also

### Assigning Intersection Function Tables

func setVertexIntersectionFunctionTables([(any MTLIntersectionFunctionTable)?], bufferRange: Range&lt;Int>)

Assigns multiple intersection function tables to a range of entries in the vertex shader argument table.

