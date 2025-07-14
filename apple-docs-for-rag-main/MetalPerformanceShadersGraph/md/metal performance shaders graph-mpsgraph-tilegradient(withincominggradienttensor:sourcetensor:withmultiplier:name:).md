

- Metal Performance Shaders Graph
- MPSGraph
-  tileGradient(withIncomingGradientTensor:sourceTensor:withMultiplier:name:) 

Instance Method

# tileGradient(withIncomingGradientTensor:sourceTensor:withMultiplier:name:)

Creates a tile gradient operation and returns the result tensor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func tileGradient(
    withIncomingGradientTensor incomingGradientTensor: MPSGraphTensor,
    sourceTensor: MPSGraphTensor,
    withMultiplier multiplier: [NSNumber],
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`incomingGradientTensor`  

The input gradient tensor.

`sourceTensor`  

The input tensor of the forward pass.

`multiplier`  

An array of numbers that specifies how many copies per dimension MPSGraph produced in the forward pass.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object.

