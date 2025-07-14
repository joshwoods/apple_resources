

- Metal Performance Shaders Graph
- MPSGraph
-  complexTensor(realTensor:imaginaryTensor:name:) 

Instance Method

# complexTensor(realTensor:imaginaryTensor:name:)

Returns a complex tensor from the two input tensors.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
func complexTensor(
    realTensor: MPSGraphTensor,
    imaginaryTensor: MPSGraphTensor,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`realTensor`  

The real part of the complex tensor.

`imaginaryTensor`  

The imaginary part of the complex tensor.

`name`  

An optional string which serves as an identifier for the operation..

## Return Value

A valid `MPSGraphTensor` object containing the elementwise result of the applied operation.

