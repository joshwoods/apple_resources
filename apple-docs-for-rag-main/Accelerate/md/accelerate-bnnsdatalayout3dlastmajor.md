

- Accelerate
-  BNNSDataLayout3DLastMajor 

Global Variable

# BNNSDataLayout3DLastMajor

A constant that represents a 3D last-major tensor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var BNNSDataLayout3DLastMajor: BNNSDataLayout { get }
```

## Discussion

The value `(i, j, k)` is at index `i * stride[0] + j * stride[1] + k * stride[2]`.

- `size[0]` is the size of the first dimension (`i`).

- `size[1]` is the size of the second dimension (`j`).

- `size[2]` is the size of the third dimension (`k`).

## See Also

### 3D Data Layouts

var BNNSDataLayoutImageCHW: BNNSDataLayout

A constant that represents a 3D image stack.

var BNNSDataLayout3DFirstMajor: BNNSDataLayout

A constant that represents a 3D first-major tensor.

var BNNSDataLayoutSNE: BNNSDataLayout

A constant that represents a 3D tensor with the size elements embedding dimension, batch size, and sequence length.

var BNNSDataLayoutNSE: BNNSDataLayout

A constant that represents a 3D tensor with the size elements embedding dimension, sequence length, and batch size.

