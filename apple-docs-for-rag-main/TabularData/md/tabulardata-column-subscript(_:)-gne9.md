

- TabularData
- Column
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Accesses a contiguous range of elements.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
subscript(bounds: Range) -> ColumnSlice { get set }
```

## Parameters 

`bounds`  

A range of valid indices in the column.

## See Also

### Accessing Elements

subscript(Int) -> Column&lt;WrappedElement>.Element

Accesses an element at an index.

subscript&lt;R>(R) -> ColumnSlice&lt;WrappedElement>

Accesses a contiguous range of elements with a range expression.

