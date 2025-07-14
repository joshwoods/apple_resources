

- TabularData
- Column
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Accesses an element at an index.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
subscript(position: Int) -> Column.Element { get set }
```

## Parameters 

`position`  

A valid index to an element in the column.

## See Also

### Accessing Elements

subscript&lt;R>(R) -> ColumnSlice&lt;WrappedElement>

Accesses a contiguous range of elements with a range expression.

subscript(Range&lt;Int>) -> ColumnSlice&lt;WrappedElement>

Accesses a contiguous range of elements.

