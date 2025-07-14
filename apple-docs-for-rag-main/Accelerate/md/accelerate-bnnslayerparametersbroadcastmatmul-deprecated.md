

- Accelerate
-  BNNSLayerParametersBroadcastMatMul Deprecated

Structure

# BNNSLayerParametersBroadcastMatMul

A set of parameters that define a broadcast matrix multiply layer.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
struct BNNSLayerParametersBroadcastMatMul
```

Deprecated

Use BNNSGraph\* APIs

## Topics

### Initializers

init(alpha: Float, beta: Float, transA: Bool, transB: Bool, quadratic: Bool, a_is_weights: Bool, b_is_weights: Bool, iA_desc: BNNSNDArrayDescriptor, iB_desc: BNNSNDArrayDescriptor, o_desc: BNNSNDArrayDescriptor)

Returns a new broadcast matrix multiply layer parameters structure from the specified parameters.

init()

Returns a new broadcast matrix multiply layer parameters structure.

### Instance Properties

var alpha: Float

A value to scale the result.

var beta: Float

A value, that must be either 0.0 or 1.0, you use to scale the existing output before the operation adds it to the result.

var transA: Bool

A Boolean value that transposes the last two dimensions of matrix *A*.

var transB: Bool

A Boolean value that transposes the last two dimensions of matrix *B*.

var quadratic: Bool

A Boolean value that determines whether the operation multiplies matrix *A* by itself.

var a_is_weights: Bool

A Boolean value that determines whether to treat matrix *A* as weights.

var b_is_weights: Bool

A Boolean value that determines whether to treat matrix *B* as weights.

var iA_desc: BNNSNDArrayDescriptor

The descriptor of matrix *A*.

var iB_desc: BNNSNDArrayDescriptor

The descriptor of matrix *B*.

var o_desc: BNNSNDArrayDescriptor

The descriptor of the output.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Matrix multiplication

func BNNSDirectApplyBroadcastMatMul(Bool, Bool, Float, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSFilterParameters>?)

Applies a broadcast matrix multiplication operation directly to two input matrices.

Deprecated

class BroadcastMatrixMultiplyLayer

A layer object that wraps a broadcast matrix multiply filter and manages its deinitialization.

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

