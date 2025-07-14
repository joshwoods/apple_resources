

- Core ML
- MLTensor
-  init(ones:scalarType:) 

Initializer

# init(ones:scalarType:)

Creates a tensor with all scalars set to ones.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
init(
    ones shape: [Int],
    scalarType: Scalar.Type = Scalar.self
) where Scalar : MLTensorScalar, Scalar : BinaryFloatingPoint, Scalar.RawSignificand : FixedWidthInteger
```

## Parameters 

`shape`  

The shape of the tensor.

`scalarType`  

The scalar type.

