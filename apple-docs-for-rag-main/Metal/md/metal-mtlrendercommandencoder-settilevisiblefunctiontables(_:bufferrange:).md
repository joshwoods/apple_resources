

- Metal
- MTLRenderCommandEncoder
-  setTileVisibleFunctionTables(\_:bufferRange:) 

Instance Method

# setTileVisibleFunctionTables(\_:bufferRange:)

Assigns multiple visible function tables to a range of entries in the tile shader argument table.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 16.0+visionOS

``` source
func setTileVisibleFunctionTables(
    _ functionTables: [(any MTLVisibleFunctionTable)?],
    bufferRange: Range
)
```

## Parameters 

`functionTables`  

An array of MTLVisibleFunctionTable instances the command assigns to entries in the tile shader argument table for visible function tables.

`bufferRange`  

A span of integers that represent the entries in the tile shader argument table for visible function tables. Each entry stores a record of the corresponding element in `functionTables`.

## Discussion

By default, the visible function table at each index is `nil`.

Note

The Objective-C version of this method is setTileVisibleFunctionTables:withBufferRange:.

## See Also

### Assigning Visible Function Tables

func setTileVisibleFunctionTable((any MTLVisibleFunctionTable)?, bufferIndex: Int)

Assigns a visible function table to an entry in the tile shader argument table.

**Required**

