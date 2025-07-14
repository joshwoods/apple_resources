

- Metal Performance Shaders Graph
- MPSGraph
-  randomTensor(withShapeTensor:descriptor:seed:name:) 

Instance Method

# randomTensor(withShapeTensor:descriptor:seed:name:)

Creates a Random op of type matching distribution in descriptor and returns random values.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func randomTensor(
    withShapeTensor shapeTensor: MPSGraphTensor,
    descriptor: MPSGraphRandomOpDescriptor,
    seed: Int,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`shapeTensor`  

1D Int32 or Int64 tensor. The shape of the tensor generated

`descriptor`  

The descriptor of the distribution. See MPSGraphRandomOpDescriptor.

`seed`  

The seed to use to initialize state. All calls with equal seed yield an identical stream of random values.

`name`  

The name for the operation.

## Return Value

An MPSGraphTensor of shape containing random values in the defined range.

## Discussion

Returns a tensor of provided shape of random values in the distribution specified. Uses the provided seed value to initalize state. No state is preserved, and all calls with equal seed yield an identical stream of random values.

