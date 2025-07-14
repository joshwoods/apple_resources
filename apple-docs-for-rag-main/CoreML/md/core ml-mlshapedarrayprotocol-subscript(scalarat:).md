

- Core ML
- MLShapedArrayProtocol
-  subscript(scalarAt:) 

Instance Subscript

# subscript(scalarAt:)

Accesses an element and a multidimensional location.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
subscript(scalarAt indices: C) -> Self.Scalar where C : Collection, C.Element == Int { get set }
```

**Required** Default implementation provided.

## Parameters 

`indices`  

An integer collection that represents a position in the shaped array in which each integer is an index in the corresponding dimension.

## Default Implementations

### MLShapedArrayProtocol Implementations

subscript(scalarAt _: Int...) -> Self.Scalar

## See Also

### Accessing Elements

subscript&lt;C>(C) -> MLShapedArraySlice&lt;Self.Scalar>

Accesses a slice using a collection of integers, in which each element is an index in the corresponding dimension.

**Required** Default implementations provided.

subscript&lt;C>(C) -> MLShapedArraySlice&lt;Self.Scalar>

Accesses a slice using a collection of integer ranges, in which each element is a range in the corresponding dimension.

**Required** Default implementations provided.

