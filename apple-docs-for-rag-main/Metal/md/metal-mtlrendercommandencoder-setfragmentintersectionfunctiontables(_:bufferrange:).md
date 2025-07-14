

- Metal
- MTLRenderCommandEncoder
-  setFragmentIntersectionFunctionTables(\_:bufferRange:) 

Instance Method

# setFragmentIntersectionFunctionTables(\_:bufferRange:)

Assigns multiple intersection function tables to a range of entries in the fragment shader argument table.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 16.0+visionOS

``` source
func setFragmentIntersectionFunctionTables(
    _ functionTables: [(any MTLIntersectionFunctionTable)?],
    bufferRange: Range
)
```

## Parameters 

`functionTables`  

An array of MTLIntersectionFunctionTable instances the command assigns to entries in the fragment shader argument table for intersection function tables.

`bufferRange`  

A span of integers that represent the entries in the fragment shader argument table for intersection function tables. Each entry stores a record of the corresponding element in `functionTables`.

## Discussion

By default, the intersection function table at each index is `nil`.

Note

The Objective-C version of this method is setFragmentIntersectionFunctionTables:withBufferRange:.

## See Also

### Assigning Intersection Function Tables

func setFragmentIntersectionFunctionTable((any MTLIntersectionFunctionTable)?, bufferIndex: Int)

Assigns an intersection function table to an entry in the fragment shader argument table.

**Required**

