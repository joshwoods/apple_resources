

- Metal Performance Shaders Graph
- MPSGraph
-  randomUniformTensor(withShapeTensor:name:) 

Instance Method

# randomUniformTensor(withShapeTensor:name:)

Creates a RandomUniform operation and returns random uniform values

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func randomUniformTensor(
    withShapeTensor shapeTensor: MPSGraphTensor,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`shapeTensor`  

1D Int32 or Int64 tensor. The shape of the tensor generated

`name`  

The name for the operation.

## Return Value

An MPSGraphTensor of shape containing random values in the defined range.

## Discussion

Returns a tensor of provided shape of random uniform values in the range \[0.0, 1.0). Uses a random seed value to initalize state. No state is preserved, and subsequent calls are not guaranteed to result in a unique stream of random values.

