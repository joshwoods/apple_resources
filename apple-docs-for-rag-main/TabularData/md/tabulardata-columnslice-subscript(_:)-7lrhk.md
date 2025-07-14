

- TabularData
- ColumnSlice
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Accesses a contiguous range of elements.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
subscript(range: Range) -> ColumnSlice { get set }
```

## Parameters 

`range`  

A range of valid indices in the column slice.

## See Also

### Accessing Elements

subscript(Int) -> ColumnSlice&lt;WrappedElement>.Element

Accesses an element at an index.

