

- Core ML
- MLShapedArrayProtocol
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Accesses a slice using a collection of integer ranges, in which each element is a range in the corresponding dimension.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
subscript(sliceRanges: C) -> MLShapedArraySlice where C : Collection, C.Element == Range { get set }
```

**Required** Default implementations provided.

## Default Implementations

### MLShapedArrayProtocol Implementations

subscript(any MLShapedArrayRangeExpression...) -> MLShapedArraySlice&lt;Self.Scalar>

subscript(Int) -> MLShapedArraySlice&lt;Self.Scalar>

subscript(any MLShapedArrayRangeExpression) -> MLShapedArraySlice&lt;Self.Scalar>

subscript(Range&lt;Int>) -> MLShapedArraySlice&lt;Self.Scalar>

subscript&lt;C>(C) -> MLShapedArraySlice&lt;Self.Scalar>

subscript((UnboundedRange_) -> Void) -> MLShapedArraySlice&lt;Self.Scalar>

subscript(Int...) -> MLShapedArraySlice&lt;Self.Scalar>

## See Also

### Accessing Elements

subscript&lt;C>(scalarAt _: C) -> Self.Scalar

Accesses an element and a multidimensional location.

**Required** Default implementation provided.

subscript&lt;C>(C) -> MLShapedArraySlice&lt;Self.Scalar>

Accesses a slice using a collection of integers, in which each element is an index in the corresponding dimension.

**Required** Default implementations provided.

