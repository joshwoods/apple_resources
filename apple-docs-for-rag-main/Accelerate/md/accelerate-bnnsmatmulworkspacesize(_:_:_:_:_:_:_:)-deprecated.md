

- Accelerate
-  BNNSMatMulWorkspaceSize(\_:\_:\_:\_:\_:\_:\_:) Deprecated

Function

# BNNSMatMulWorkspaceSize(\_:\_:\_:\_:\_:\_:\_:)

Returns the workspace size that a matrix multiply operation requires.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 9.0–11.0Deprecated

``` source
func BNNSMatMulWorkspaceSize(
    _ transA: Bool,
    _ transB: Bool,
    _ alpha: Float,
    _ inputA: UnsafePointer,
    _ inputB: UnsafePointer,
    _ output: UnsafePointer,
    _ filter_params: UnsafePointer?
) -> Int
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`transA`  

A Boolean value that specifies whether the operation should treat `inputA` as transposed.

`transB`  

A Boolean value that specifies whether the operation should treat `inputB` as transposed.

`alpha`  

A value that the operation uses to scale the result.

`inputA`  

A pointer to the `inputA` matrix descriptor.

`inputB`  

A pointer to the `inputB` matrix descriptor.

`output`  

A pointer to the output matrix descriptor.

`filter_params`  

The filter runtime parameters.

## Return Value

The required allocation size for workspace paramter to BNNSMatMul(_:_:_:_:_:_:_:_:), in bytes.

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

func BNNSMatMul(Bool, Bool, Float, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafeMutableRawPointer?, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Applies a matrix multiplication operation directly to two input matrices.

Deprecated

static func applyMatrixMultiplication(inputA: BNNSNDArrayDescriptor, transposed: Bool, inputB: BNNSNDArrayDescriptor, transposed: Bool, output: BNNSNDArrayDescriptor, alpha: Float, workspace: UnsafeMutableRawBufferPointer?, filterParameters: BNNSFilterParameters?) throws

Performs a matrix multiplication operation directly on two input matrices.

Deprecated

static func matrixMultiplicationWorkspaceSize(inputA: BNNSNDArrayDescriptor, transposed: Bool, inputB: BNNSNDArrayDescriptor, transposed: Bool, output: BNNSNDArrayDescriptor, alpha: Float, filterParameters: BNNSFilterParameters?) -> Int?

Returns the workspace size that a matrix multiply operation requires.

Deprecated

