

- Metal Performance Shaders Graph
- MPSGraph
-  resizeBilinear(withGradientTensor:input:scaleOffsetTensor:layout:name:) 

Instance Method

# resizeBilinear(withGradientTensor:input:scaleOffsetTensor:layout:name:)

Creates a Resize gradient operation and returns the result tensor.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func resizeBilinear(
    withGradientTensor gradient: MPSGraphTensor,
    input: MPSGraphTensor,
    scaleOffsetTensor scaleOffset: MPSGraphTensor,
    layout: MPSGraphTensorNamedDataLayout,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`gradient`  

Incoming gradient tensor

`input`  

Forward pass input tensor

`scaleOffset`  

1D float tensor. A 4-element shape as \[scaleY, scaleX, offsetY, offsetX\]

`layout`  

Specifies what layout the provided tensor is in. The returned tensor will follow the same layout. Valid layouts are NHWC, NCHW, HWC, CHW, and HW.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object

## Discussion

Computes the gradient for the forward pass Resize op with bilinear sampling and identical parameters. See discussion of resizeTensor for more in depth description of resize paramters.

