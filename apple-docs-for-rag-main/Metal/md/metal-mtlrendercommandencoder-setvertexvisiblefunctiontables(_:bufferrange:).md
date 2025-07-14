

- Metal
- MTLRenderCommandEncoder
-  setVertexVisibleFunctionTables(\_:bufferRange:) 

Instance Method

# setVertexVisibleFunctionTables(\_:bufferRange:)

Assigns multiple visible function tables to a range of entries in the vertex shader argument table.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 16.0+visionOS

``` source
func setVertexVisibleFunctionTables(
    _ functionTables: [(any MTLVisibleFunctionTable)?],
    bufferRange: Range
)
```

## Parameters 

`functionTables`  

An array of MTLVisibleFunctionTable instances the command assigns to entries in the vertex shader argument table for visible function tables.

`bufferRange`  

A span of integers that represent the entries in the vertex shader argument table for visible function tables. Each entry stores a record of the corresponding element in `functionTables`.

## Discussion

By default, the visible function table at each index is `nil`.

Note

The Objective-C version of this method is setVertexVisibleFunctionTables:withBufferRange:.

## See Also

### Assigning Visible Function Tables

func setVertexVisibleFunctionTable((any MTLVisibleFunctionTable)?, bufferIndex: Int)

Assigns a visible function table to an entry in the vertex shader argument table.

**Required**

