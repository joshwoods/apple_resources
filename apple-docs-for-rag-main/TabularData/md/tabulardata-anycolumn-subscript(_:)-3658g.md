

- TabularData
- AnyColumn
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Returns a slice of the column by selecting elements with a collection of Booleans.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
subscript(mask: C) -> AnyColumnSlice where C : Collection, C.Element == Bool { get }
```

## Parameters 

`mask`  

A collection of Booleans. The method selects the column’s elements that correspond to the `true` elements in the collection.

