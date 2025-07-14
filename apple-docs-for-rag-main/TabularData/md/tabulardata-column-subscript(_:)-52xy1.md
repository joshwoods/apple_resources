

- TabularData
- Column
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Accesses a contiguous range of elements with a range expression.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
subscript(range: R) -> ColumnSlice where R : RangeExpression, R.Bound == Int { get set }
```

## Parameters 

`range`  

An integer range expression that represents valid indices in the column.

## See Also

### Accessing Elements

subscript(Int) -> Column&lt;WrappedElement>.Element

Accesses an element at an index.

subscript(Range&lt;Int>) -> ColumnSlice&lt;WrappedElement>

Accesses a contiguous range of elements.

