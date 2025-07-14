

- Metal Performance Shaders Graph
- MPSGraph
-  stack(\_:axis:name:) 

Instance Method

# stack(\_:axis:name:)

Creates a stack operation and returns the result tensor.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 12.3+tvOS 15.4+visionOS 1.0+

``` source
func stack(
    _ inputTensors: [MPSGraphTensor],
    axis: Int,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`inputTensors`  

The input tensors.

`axis`  

The dimension to stack tensors into result. Must be in range: `-rank + 1 

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object.

## Discussion

Stacks all input tensors along `axis` into a result tensor of `rank + 1`. Tensors must be broadcast compatible along all dimensions except `axis`, and have the same type.

