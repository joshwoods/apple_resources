

- Metal
- MTLRenderCommandEncoder
-  setFragmentIntersectionFunctionTable(\_:bufferIndex:) 

Instance Method

# setFragmentIntersectionFunctionTable(\_:bufferIndex:)

Assigns an intersection function table to an entry in the fragment shader argument table.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
func setFragmentIntersectionFunctionTable(
    _ intersectionFunctionTable: (any MTLIntersectionFunctionTable)?,
    bufferIndex: Int
)
```

**Required**

## Parameters 

`intersectionFunctionTable`  

An MTLIntersectionFunctionTable instance the command assigns to an entry in the fragment shader argument table for intersection function tables.

`bufferIndex`  

An integer that represents the entry in the fragment shader argument table for intersection function tables that stores a record of `intersectionFunctionTable`.

## Discussion

By default, the intersection function table at each index is `nil`.

## See Also

### Assigning Intersection Function Tables

func setFragmentIntersectionFunctionTables([(any MTLIntersectionFunctionTable)?], bufferRange: Range&lt;Int>)

Assigns multiple intersection function tables to a range of entries in the fragment shader argument table.

