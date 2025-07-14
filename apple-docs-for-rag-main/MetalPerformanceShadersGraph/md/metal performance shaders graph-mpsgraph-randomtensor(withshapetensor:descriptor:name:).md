

- Metal Performance Shaders Graph
- MPSGraph
-  randomTensor(withShapeTensor:descriptor:name:) 

Instance Method

# randomTensor(withShapeTensor:descriptor:name:)

Creates a Random op of type matching distribution in descriptor and returns random values.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func randomTensor(
    withShapeTensor shapeTensor: MPSGraphTensor,
    descriptor: MPSGraphRandomOpDescriptor,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`shapeTensor`  

1D Int32 or Int64 tensor. The shape of the tensor generated

`descriptor`  

The descriptor of the distribution. See MPSGraphRandomOpDescriptor.

`name`  

The name for the operation.

## Return Value

An MPSGraphTensor of shape containing random values in the defined range.

## Discussion

Returns a tensor of provided shape of random values in the distribution specified. Uses a random seed value to initalize state. No state is preserved, and subsequent calls are not guaranteed to result in a unique stream of random values.

