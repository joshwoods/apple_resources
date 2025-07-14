

- Metal
- MTLRenderCommandEncoder
-  setTileVisibleFunctionTable(\_:bufferIndex:) 

Instance Method

# setTileVisibleFunctionTable(\_:bufferIndex:)

Assigns a visible function table to an entry in the tile shader argument table.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
func setTileVisibleFunctionTable(
    _ functionTable: (any MTLVisibleFunctionTable)?,
    bufferIndex: Int
)
```

**Required**

## Parameters 

`functionTable`  

An MTLVisibleFunctionTable instance the command assigns to an entry in the tile shader argument table for visible function tables.

`bufferIndex`  

An integer that represents the entry in the tile shader argument table for visible function tables that stores a record of `functionTable`.

## Discussion

By default, the visible function table at each index is `nil`.

## See Also

### Assigning Visible Function Tables

func setTileVisibleFunctionTables([(any MTLVisibleFunctionTable)?], bufferRange: Range&lt;Int>)

Assigns multiple visible function tables to a range of entries in the tile shader argument table.

