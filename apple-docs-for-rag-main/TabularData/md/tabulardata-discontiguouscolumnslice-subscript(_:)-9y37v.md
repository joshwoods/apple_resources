

- TabularData
- DiscontiguousColumnSlice
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Accesses an element at an index.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
subscript(position: Int) -> DiscontiguousColumnSlice.Element { get set }
```

## Parameters 

`position`  

A valid index to an element in the column slice.

## See Also

### Accessing Elements

subscript(Range&lt;Int>) -> DiscontiguousColumnSlice&lt;WrappedElement>

Accesses a contiguous range of elements.

subscript&lt;R>(R) -> DiscontiguousColumnSlice&lt;WrappedElement>

Accesses a contiguous range of elements with a range expression.

subscript((UnboundedRange_) -> ()) -> DiscontiguousColumnSlice&lt;WrappedElement>

Accesses a contiguous range of elements with an unbounded range.

