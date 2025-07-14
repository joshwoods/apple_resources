

- Core ML
- MLTensor
-  init(repeating:shape:scalarType:) 

Initializer

# init(repeating:shape:scalarType:)

Creates a tensor with the specified shape and a single, repeated scalar value.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
init(
    repeating repeatedValue: Scalar,
    shape: [Int],
    scalarType: Scalar.Type = Scalar.self
) where Scalar : MLTensorScalar
```

## Parameters 

`repeatedValue`  

The scalar value to repeat.

`shape`  

The shape of the tensor.

`scalarType`  

The scalar type.

