

- Accelerate
-  BNNSDataLayoutRowMajorMatrix 

Global Variable

# BNNSDataLayoutRowMajorMatrix

A constant that represents a 2D row-major matrix.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var BNNSDataLayoutRowMajorMatrix: BNNSDataLayout { get }
```

## Discussion

The value `(row, col)` is at index `col * stride[0] + row * stride[1]`.

- `size[0]` is the number of columns.

- `size[1]` is the number of rows.

## See Also

### 2D Data Layouts

var BNNSDataLayoutColumnMajorMatrix: BNNSDataLayout

A constant that represents a 2D column-major matrix.

var BNNSDataLayout2DFirstMajor: BNNSDataLayout

A constant that represents a 2D first-major matrix.

var BNNSDataLayout2DLastMajor: BNNSDataLayout

A constant that represents a 2D last-major matrix.

