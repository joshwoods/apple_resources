

- Metal Performance Shaders Graph
- MPSGraph
-  padGradient(withIncomingGradientTensor:sourceTensor:paddingMode:leftPadding:rightPadding:name:) 

Instance Method

# padGradient(withIncomingGradientTensor:sourceTensor:paddingMode:leftPadding:rightPadding:name:)

Creates a padding gradient operation and returns the result tensor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func padGradient(
    withIncomingGradientTensor incomingGradientTensor: MPSGraphTensor,
    sourceTensor: MPSGraphTensor,
    paddingMode: MPSGraphPaddingMode,
    leftPadding: [NSNumber],
    rightPadding: [NSNumber],
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`incomingGradientTensor`  

The input gradient tensor.

`sourceTensor`  

The input tensor of the forward pass.

`paddingMode`  

The parameter that defines the padding mode.

`leftPadding`  

The parameter that defines how much padding the operation applies to the input tensor before each dimension - must be of size `rank(tensor)`.

`rightPadding`  

The parameter that defines how much padding the operation applies to the input tensor after each dimension - must be of size `rank(tensor)`.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object.

