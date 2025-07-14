

- Accelerate
- BNNS
-  matrixMultiplicationWorkspaceSize(inputA:transposed:inputB:transposed:output:alpha:filterParameters:) Deprecated

Type Method

# matrixMultiplicationWorkspaceSize(inputA:transposed:inputB:transposed:output:alpha:filterParameters:)

Returns the workspace size that a matrix multiply operation requires.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
static func matrixMultiplicationWorkspaceSize(
    inputA: BNNSNDArrayDescriptor,
    transposed transposeA: Bool,
    inputB: BNNSNDArrayDescriptor,
    transposed transposeB: Bool,
    output: BNNSNDArrayDescriptor,
    alpha: Float,
    filterParameters: BNNSFilterParameters? = nil
) -> Int?
```

Deprecated

Use the BNNSGraph API instead.

## Parameters 

`inputA`  

The descriptor of matrix A.

`transposeA`  

A Boolean value that indicates whether the function transposes the last two dimensions of matrix A.

`inputB`  

The descriptor of matrix B.

`transposeB`  

A Boolean value that indicates whether the function transposes the last two dimensions of matrix B\_.\_

`output`  

The descriptor of the output.

`alpha`  

A scalar value that scales the result.

`filterParameters`  

The filter runtime parameters.

## See Also

### Matrix multiplication

func BNNSDirectApplyBroadcastMatMul(Bool, Bool, Float, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSFilterParameters>?)

Applies a broadcast matrix multiplication operation directly to two input matrices.

Deprecated

class BroadcastMatrixMultiplyLayer

A layer object that wraps a broadcast matrix multiply filter and manages its deinitialization.

Deprecated

struct BNNSLayerParametersBroadcastMatMul

A set of parameters that define a broadcast matrix multiply layer.

Deprecated

func BNNSFilterCreateLayerBroadcastMatMul(UnsafePointer&lt;BNNSLayerParametersBroadcastMatMul>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new broadcast matrix multiply layer.

Deprecated

func BNNSMatMulWorkspaceSize(Bool, Bool, Float, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSFilterParameters>?) -> Int

Returns the workspace size that a matrix multiply operation requires.

Deprecated

func BNNSMatMul(Bool, Bool, Float, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafeMutableRawPointer?, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Applies a matrix multiplication operation directly to two input matrices.

Deprecated

static func applyMatrixMultiplication(inputA: BNNSNDArrayDescriptor, transposed: Bool, inputB: BNNSNDArrayDescriptor, transposed: Bool, output: BNNSNDArrayDescriptor, alpha: Float, workspace: UnsafeMutableRawBufferPointer?, filterParameters: BNNSFilterParameters?) throws

Performs a matrix multiplication operation directly on two input matrices.

Deprecated

