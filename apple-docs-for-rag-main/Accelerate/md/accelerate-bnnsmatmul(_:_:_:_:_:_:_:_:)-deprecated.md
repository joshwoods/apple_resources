

- Accelerate
-  BNNSMatMul(\_:\_:\_:\_:\_:\_:\_:\_:) Deprecated

Function

# BNNSMatMul(\_:\_:\_:\_:\_:\_:\_:\_:)

Applies a matrix multiplication operation directly to two input matrices.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 9.0–11.0Deprecated

``` source
func BNNSMatMul(
    _ transA: Bool,
    _ transB: Bool,
    _ alpha: Float,
    _ inputA: UnsafePointer,
    _ inputB: UnsafePointer,
    _ output: UnsafePointer,
    _ workspace: UnsafeMutableRawPointer?,
    _ filter_params: UnsafePointer?
) -> Int32
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

`workspace`  

An optional pointer to the workspace memory. Use BNNSMatMulWorkspaceSize(_:_:_:_:_:_:_:) to calculate the workspace size that operation requires. BNNSMatMul(_:_:_:_:_:_:_:_:) doesn’t require any particular alignment for the workspace memory.

`filter_params`  

The filter runtime parameters.

## Discussion

Use this function to perform the operation `C = alpha * op(A) * op(B)` where `op` transposes the corresponding matrix if the appropriate transpose parameter is `true`. The function broadcasts dimensions that are absent on either input matrix. The matrix multiplication is always on the final two indices of each operand.

For example, the following arrays of values and descriptors for the matrix multiply inputs and outputs define a matrix multiplication operation without broadcasting. Note that the operation repeats the values in `inputBValues` along the third dimension.

```
let inputAValues: [Float] = [
    [ 24 values ]
]

let inputBValues: [Float] = [
    1, 2,
    3, 4,

    1, 2,
    3, 4,

    1, 2,
    3, 4
]

var inputADescriptor = BNNSNDArrayDescriptor.allocate(
    initializingFrom: inputAValues,
    shape: .imageCHW(3, 4, 2))

var inputBDescriptor = BNNSNDArrayDescriptor.allocate(
    initializingFrom: inputBValues,
    shape: .tensor3DFirstMajor(3, 2, 2))

var outputDescriptor = BNNSNDArrayDescriptor.allocateUninitialized(
    scalarType: Float.self,
    shape: .imageCHW(inputADescriptor.shape.size.0,
                     inputADescriptor.shape.size.1,
                     inputBDescriptor.shape.size.1))
```

The BNNSMatMul(_:_:_:_:_:_:_:_:) function calculates the same result using a 2 x 2 matrix.

```
let inputBValues: [Float] = [
    1, 2,
    3, 4
]

var inputBDescriptor = BNNSNDArrayDescriptor.allocate(
    initializingFrom: inputBValues,
    shape: .matrixFirstMajor(2, 2))
```

In both cases, the call to the matrix multiply function is the same.

```
BNNSMatMul(false, false,
           1,
           &inputADescriptor, &inputBDescriptor,
           &outputDescriptor,
           nil, nil)
```

You may optionally pass a workspace to BNNSMatMul(_:_:_:_:_:_:_:_:). Call BNNSMatMulWorkspaceSize(_:_:_:_:_:_:_:) to calculate the required workspace size for a set of parameters. If you pass `nil` to the BNNSMatMul(_:_:_:_:_:_:_:_:) workspace parameter, BNNS allocates and dellocates the workspace.

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

static func applyMatrixMultiplication(inputA: BNNSNDArrayDescriptor, transposed: Bool, inputB: BNNSNDArrayDescriptor, transposed: Bool, output: BNNSNDArrayDescriptor, alpha: Float, workspace: UnsafeMutableRawBufferPointer?, filterParameters: BNNSFilterParameters?) throws

Performs a matrix multiplication operation directly on two input matrices.

Deprecated

static func matrixMultiplicationWorkspaceSize(inputA: BNNSNDArrayDescriptor, transposed: Bool, inputB: BNNSNDArrayDescriptor, transposed: Bool, output: BNNSNDArrayDescriptor, alpha: Float, filterParameters: BNNSFilterParameters?) -> Int?

Returns the workspace size that a matrix multiply operation requires.

Deprecated

