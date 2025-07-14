

- Metal Performance Shaders Graph
- MPSGraph
-  split(\_:splitSizes:axis:name:) 

Instance Method

# split(\_:splitSizes:axis:name:)

Creates a split operation and returns the result tensor.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 12.3+tvOS 15.4+visionOS 1.0+

``` source
func split(
    _ tensor: MPSGraphTensor,
    splitSizes: [NSNumber],
    axis: Int,
    name: String?
) -> [MPSGraphTensor]
```

## Parameters 

`tensor`  

The input tensor.

`splitSizes`  

The lengths of the result tensors along the split axis.

`axis`  

The dimension along which MPSGraph splits the input tensor.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object.

## Discussion

Splits the input tensor along `axis` into multiple result tensors of size determined by `splitSizes`. Requires that the sum of `splitSizes` is equal to the lenth of the input along `axis`.

