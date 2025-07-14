

- Metal Performance Shaders Graph
- MPSGraph
-  resize(\_:sizeTensor:scaleOffsetTensor:mode:layout:name:) 

Instance Method

# resize(\_:sizeTensor:scaleOffsetTensor:mode:layout:name:)

Resamples input images to given size using the provided scale and offset. Destination indices are computed using

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func resize(
    _ imagesTensor: MPSGraphTensor,
    sizeTensor size: MPSGraphTensor,
    scaleOffsetTensor scaleOffset: MPSGraphTensor,
    mode: MPSGraphResizeMode,
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

`mode`  

The resampling mode to use. If nearest sampling is specifed, RoundPreferCeil mode will be used.

`layout`  

Specifies what layout the provided tensor is in. The returned tensor will follow the same layout. Valid layouts are NHWC, NCHW, HWC, CHW, and HW.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object

## Discussion

```
dst_indices = (src_indicesscale) + offset 
```

For most use cases passing the scale and offset directly is unnecessary, and it is preferable to use the API specifying centerResult and alignCorners.

