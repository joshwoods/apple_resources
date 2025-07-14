

- TabularData
- DiscontiguousColumnSlice
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Accesses a contiguous range of elements.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
subscript(range: Range) -> DiscontiguousColumnSlice { get set }
```

## Parameters 

`range`  

A range of valid indices in the column slice.

## See Also

### Accessing Elements

subscript(Int) -> DiscontiguousColumnSlice&lt;WrappedElement>.Element

Accesses an element at an index.

subscript&lt;R>(R) -> DiscontiguousColumnSlice&lt;WrappedElement>

Accesses a contiguous range of elements with a range expression.

subscript((UnboundedRange_) -> ()) -> DiscontiguousColumnSlice&lt;WrappedElement>

Accesses a contiguous range of elements with an unbounded range.

