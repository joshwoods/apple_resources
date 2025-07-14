

- Accelerate
-  BNNSDataLayoutImageCHW 

Global Variable

# BNNSDataLayoutImageCHW

A constant that represents a 3D image stack.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var BNNSDataLayoutImageCHW: BNNSDataLayout { get }
```

## Discussion

The value `(x, y, channel)` is at index `x * stride[0] + y * stride[1] + channel * stride[2]`.

- `size[0]` is the image width in pixels.

- `size[1]` is the image height in pixels.

- `size[2]` is the number of channels.

## See Also

### 3D Data Layouts

var BNNSDataLayout3DFirstMajor: BNNSDataLayout

A constant that represents a 3D first-major tensor.

var BNNSDataLayout3DLastMajor: BNNSDataLayout

A constant that represents a 3D last-major tensor.

var BNNSDataLayoutSNE: BNNSDataLayout

A constant that represents a 3D tensor with the size elements embedding dimension, batch size, and sequence length.

var BNNSDataLayoutNSE: BNNSDataLayout

A constant that represents a 3D tensor with the size elements embedding dimension, sequence length, and batch size.

