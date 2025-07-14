

- Core ML
- MLTensor
-  shapedArray(of:) 

Instance Method

# shapedArray(of:)

Returns a materialized representation of the tensor.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func shapedArray(of scalarType: Scalar.Type) async -> MLShapedArray where Scalar : MLShapedArrayScalar, Scalar : MLTensorScalar
```

## Return Value

A `MLShapedArray` with the contents of the tensor.

