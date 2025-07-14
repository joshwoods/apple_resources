

- Metal
- MTLRenderCommandEncoder
-  setTileIntersectionFunctionTables(\_:bufferRange:) 

Instance Method

# setTileIntersectionFunctionTables(\_:bufferRange:)

Assigns multiple intersection function tables to a range of entries in the tile shader argument table.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 16.0+visionOS

``` source
func setTileIntersectionFunctionTables(
    _ functionTables: [(any MTLIntersectionFunctionTable)?],
    bufferRange: Range
)
```

## Parameters 

`functionTables`  

An array of MTLIntersectionFunctionTable instances the command assigns to entries in the tile shader argument table for intersection function tables.

`bufferRange`  

A span of integers that represent the entries in the tile shader argument table for intersection function tables. Each entry stores a record of the corresponding element in `functionTables`.

## Discussion

By default, the intersection function table at each index is `nil`.

Note

The Objective-C version of this method is setTileIntersectionFunctionTables:withBufferRange:.

## See Also

### Assigning Intersection Function Tables

func setTileIntersectionFunctionTable((any MTLIntersectionFunctionTable)?, bufferIndex: Int)

Assigns an intersection function table to an entry in the tile shader argument table.

**Required**

