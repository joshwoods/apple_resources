

- Accelerate
-  BNNSDataLayout7DLastMajor 

Global Variable

# BNNSDataLayout7DLastMajor

A constant that represents a 7D last-major tensor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var BNNSDataLayout7DLastMajor: BNNSDataLayout { get }
```

## Discussion

The value `(i, j, k, l, m, n, o)` is at index:

`i * stride[0] + j * stride[1] + k * stride[2] + l * stride[3] +`

`m * stride[4] + n * stride[5] + o * stride[6]`.

- `size[0]` is the size of the first dimension (`i`).

- `size[1]` is the size of the second dimension (`j`).

- `size[2]` is the size of the third dimension (`k`).

- `size[3]` is the size of the fourth dimension (`l`).

- `size[4]` is the size of the fifth dimension (`m`).

- `size[5]` is the size of the sixth dimension (`n`).

- `size[6]` is the size of the seventh dimension (`o`).

## See Also

### 7D Data Layouts

var BNNSDataLayout7DFirstMajor: BNNSDataLayout

A constant that represents a 7D first-major tensor.

