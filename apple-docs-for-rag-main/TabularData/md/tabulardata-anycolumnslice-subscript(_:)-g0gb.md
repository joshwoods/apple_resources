

- TabularData
- AnyColumnSlice
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Accesses an element at an index.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
subscript(position: Int) -> Any? { get set }
```

## Parameters 

`position`  

A valid index to an element in the column slice.

## See Also

### Accessing Elements

subscript(Range&lt;Int>) -> AnyColumnSlice

Accesses a contiguous range of elements.

