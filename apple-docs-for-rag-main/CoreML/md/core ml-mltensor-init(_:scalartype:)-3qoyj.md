

- Core ML
- MLTensor
-  init(\_:scalarType:) 

Initializer

# init(\_:scalarType:)

Creates a one-dimensional tensor from scalars.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
init(
    _ scalars: some Collection,
    scalarType: Scalar.Type = Scalar.self
) where Scalar : MLTensorScalar
```

## Parameters 

`scalars`  

A collection of scalars.

`scalarType`  

The scalar type.

