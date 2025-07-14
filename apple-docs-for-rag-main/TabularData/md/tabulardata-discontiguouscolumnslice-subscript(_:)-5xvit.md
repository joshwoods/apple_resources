

- TabularData
- DiscontiguousColumnSlice
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Accesses a contiguous range of elements with an unbounded range.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
subscript(range: (UnboundedRange_) -> ()) -> DiscontiguousColumnSlice { get set }
```

## Parameters 

`range`  

An unbounded range of valid indices in the column slice.

## See Also

### Accessing Elements

subscript(Int) -> DiscontiguousColumnSlice&lt;WrappedElement>.Element

Accesses an element at an index.

subscript(Range&lt;Int>) -> DiscontiguousColumnSlice&lt;WrappedElement>

Accesses a contiguous range of elements.

subscript&lt;R>(R) -> DiscontiguousColumnSlice&lt;WrappedElement>

Accesses a contiguous range of elements with a range expression.

