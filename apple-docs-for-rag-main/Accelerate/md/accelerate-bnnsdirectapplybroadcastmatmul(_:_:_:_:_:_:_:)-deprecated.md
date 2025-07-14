

- Accelerate
-  BNNSDirectApplyBroadcastMatMul(\_:\_:\_:\_:\_:\_:\_:) Deprecated

Function

# BNNSDirectApplyBroadcastMatMul(\_:\_:\_:\_:\_:\_:\_:)

Applies a broadcast matrix multiplication operation directly to two input matrices.

iOS 14.0–16.0DeprecatediPadOS 14.0–16.0DeprecatedMac Catalyst 14.0–16.0DeprecatedmacOS 11.0–13.0DeprecatedtvOS 14.0–16.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 7.0–9.0Deprecated

``` source
func BNNSDirectApplyBroadcastMatMul(
    _ transA: Bool,
    _ transB: Bool,
    _ alpha: Float,
    _ inputA: UnsafePointer,
    _ inputB: UnsafePointer,
    _ output: UnsafePointer,
    _ filter_params: UnsafePointer?
)
```

Deprecated

Use BNNSMatMul(_:_:_:_:_:_:_:_:) instead.

## Parameters 

`transA`  

A Boolean value that transposes the last two dimensions of matrix *A*.

`transB`  

A Boolean value that transposes the last two dimensions of matrix *B*.

`alpha`  

A value to scale the result.

`inputA`  

The descriptor of matrix *A*.

`inputB`  

The descriptor of matrix *B*.

`output`  

The descriptor of the output.

`filter_params`  

The filter runtime parameters.

## See Also

### Matrix multiplication

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

static func matrixMultiplicationWorkspaceSize(inputA: BNNSNDArrayDescriptor, transposed: Bool, inputB: BNNSNDArrayDescriptor, transposed: Bool, output: BNNSNDArrayDescriptor, alpha: Float, filterParameters: BNNSFilterParameters?) -> Int?

Returns the workspace size that a matrix multiply operation requires.

Deprecated

