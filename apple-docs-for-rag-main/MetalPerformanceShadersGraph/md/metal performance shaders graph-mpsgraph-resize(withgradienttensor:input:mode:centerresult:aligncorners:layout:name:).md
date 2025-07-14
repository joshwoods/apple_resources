

- Metal Performance Shaders Graph
- MPSGraph
-  resize(withGradientTensor:input:mode:centerResult:alignCorners:layout:name:) 

Instance Method

# resize(withGradientTensor:input:mode:centerResult:alignCorners:layout:name:)

Creates a Resize gradient operation and returns the result tensor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func resize(
    withGradientTensor gradient: MPSGraphTensor,
    input: MPSGraphTensor,
    mode: MPSGraphResizeMode,
    centerResult: Bool,
    alignCorners: Bool,
    layout: MPSGraphTensorNamedDataLayout,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`gradient`  

Incoming gradient tensor

`input`  

Forward pass input tensor

`mode`  

The resampling mode to use. If nearest sampling is specifed, RoundPreferCeil mode will be used.

`centerResult`  

Controls if the result image is centered on the input image. When NO, the result will have the top left corner aligned

`alignCorners`  

When YES, the result image will have the same value as the input image in the corners

`layout`  

Specifies what layout the provided tensor is in. The returned tensor will follow the same layout. Valid layouts are NHWC, NCHW, HWC, CHW, and HW.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object

## Discussion

Computes the gradient for the forward pass Resize op with identical parameters. See discussion of resizeTensor for more in depth description of resize paramters.

