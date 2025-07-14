

- Metal Performance Shaders Graph
- MPSGraph
-  resizeBilinear(\_:sizeTensor:scaleOffsetTensor:layout:name:) 

Instance Method

# resizeBilinear(\_:sizeTensor:scaleOffsetTensor:layout:name:)

Resamples input images to given size using the provided scale and offset and bilinear sampling See above discussion for more details.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func resizeBilinear(
    _ imagesTensor: MPSGraphTensor,
    sizeTensor size: MPSGraphTensor,
    scaleOffsetTensor scaleOffset: MPSGraphTensor,
    layout: MPSGraphTensorNamedDataLayout,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`imagesTensor`  

Tensor containing input images.

`size`  

1D Int32 or Int64 tensor. A 2-element shape as \[newHeight, newWidth\]

`scaleOffset`  

1D float tensor. A 4-element shape as \[scaleY, scaleX, offsetY, offsetX\]

`layout`  

Specifies what layout the provided tensor is in. The returned tensor will follow the same layout. Valid layouts are NHWC, NCHW, HWC, CHW, and HW.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object

