

- Accelerate
-  BNNSDataLayoutNSE 

Global Variable

# BNNSDataLayoutNSE

A constant that represents a 3D tensor with the size elements embedding dimension, sequence length, and batch size.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var BNNSDataLayoutNSE: BNNSDataLayout { get }
```

## Discussion

The value `(e, s, n)` is at index `e * stride[0] + s * stride[1] + n * stride[2]`.

- `size[0]` is the embedding dimension (`e`).

- `size[1]` is the sequence length (`s`).

- `size[2]` is the batch size (`n`).

## See Also

### 3D Data Layouts

var BNNSDataLayoutImageCHW: BNNSDataLayout

A constant that represents a 3D image stack.

var BNNSDataLayout3DFirstMajor: BNNSDataLayout

A constant that represents a 3D first-major tensor.

var BNNSDataLayout3DLastMajor: BNNSDataLayout

A constant that represents a 3D last-major tensor.

var BNNSDataLayoutSNE: BNNSDataLayout

A constant that represents a 3D tensor with the size elements embedding dimension, batch size, and sequence length.

