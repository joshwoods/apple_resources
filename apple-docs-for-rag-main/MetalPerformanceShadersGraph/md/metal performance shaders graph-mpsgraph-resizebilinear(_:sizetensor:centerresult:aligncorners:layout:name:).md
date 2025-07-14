

- Metal Performance Shaders Graph
- MPSGraph
-  resizeBilinear(\_:sizeTensor:centerResult:alignCorners:layout:name:) 

Instance Method

# resizeBilinear(\_:sizeTensor:centerResult:alignCorners:layout:name:)

Resamples input images to given size using bilinear sampling.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func resizeBilinear(
    _ imagesTensor: MPSGraphTensor,
    sizeTensor size: MPSGraphTensor,
    centerResult: Bool,
    alignCorners: Bool,
    layout: MPSGraphTensorNamedDataLayout,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`imagesTensor`  

Tensor containing input images.

`size`  

1D Int32 or Int64 tensor. A 2-element shape as \[newHeight, newWidth\]

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

Resamples input images to given size using nearest neighbor sampling. Result images will be distorted if size is of different aspect ratio. Destination indices are computed using direct index scaling by default, with no offset added. If the centerResult parameter is true, the destination indices will be scaled and shifted to be centered on the input image. If the alignCorners parameter is true, the corners of the result images will match the input images. Scaling will be modified to a factor of (size - 1) / (inputSize - 1). When alignCorners is true, the centerResult parameter does nothing. In order to achieve the same behavior as OpenCV’s resize and TensorFlowV2’s resize,

```
centerResult = YES;
alginCorners = NO;
```

To achieve the same behavior as TensorFlowV1 resize

```
centerResult = NO;
```

