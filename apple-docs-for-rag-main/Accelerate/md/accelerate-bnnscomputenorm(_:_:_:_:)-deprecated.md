

- Accelerate
-  BNNSComputeNorm(\_:\_:\_:\_:) Deprecated

Function

# BNNSComputeNorm(\_:\_:\_:\_:)

Computes the specified norm over an entire tensor or the specified axes.

iOS 15.0–18.0DeprecatediPadOS 15.0–18.0DeprecatedMac Catalyst 15.0–18.0DeprecatedmacOS 12.0–15.0DeprecatedtvOS 15.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 8.0–11.0Deprecated

``` source
func BNNSComputeNorm(
    _ dest: UnsafeMutablePointer,
    _ src: UnsafePointer,
    _ norm_type: BNNSNormType,
    _ axis_flags: UInt32
) -> Int32
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`dest`  

The descriptor of the output.

`src`  

The descriptor of the input.

`norm_type`  

The type of the norm. This function supports only BNNSL2Norm.

`axis_flags`  

The dimensions that the function uses to compute the norm. Set to `0` to specify that the function computes the norm over all dimensions.

## Discussion

Use this function to compute the norm of either an entire tensor or the axis or axes of a tensor.

For example, the following code defines a 3D tensor:

```
let inputData = UnsafeMutableBufferPointer.allocate(capacity: 24)
_ = inputData.initialize(from: [1, 2, 3,
                                4, 5, 6,

                                10, 20, 30,
                                40, 50, 60,

                                100, 200, 300,
                                400, 500, 600,

                                1000, 2000, 3000,
                                4000, 5000, 6000])
var inputDescriptor = BNNSNDArrayDescriptor(flags: BNNSNDArrayFlags(0),
                                            layout: BNNSDataLayoutImageCHW,
                                            size: (3, 2, 4, 0, 0, 0, 0, 0),
                                            stride: (0, 0, 0, 0, 0, 0, 0, 0),
                                            data: inputData.baseAddress!,
                                            data_type: BNNSDataType.float,
                                            table_data: nil,
                                            table_data_type: BNNSDataType.float,
                                            data_scale: 1, data_bias: 0)
```

Define the `axis_flags` parameter as either `0b111` or `0` to specify that the operation computes the norm of the entire tensor. In this case, the norm is a scalar value, and the destination’s data layout must be a `BNNSDataLayoutVector` with a size of `1`.

```
let outputData = UnsafeMutableBufferPointer.allocate(capacity: 1)
var outputDescriptor = BNNSNDArrayDescriptor(flags: BNNSNDArrayFlags(0),
                                             layout: BNNSDataLayoutVector,
                                             size: (1, 0, 0, 0, 0, 0, 0, 0),
                                             stride: (0, 0, 0, 0, 0, 0, 0, 0),
                                             data: outputData.baseAddress!,
                                             data_type: BNNSDataType.float,
                                             table_data: nil,
                                             table_data_type: BNNSDataType.float,
                                             data_scale: 1, data_bias: 0)

BNNSComputeNorm(&outputDescriptor,
                 &inputDescriptor,
                 BNNSL2Norm,
                 0b111)

// Prints `[9587.45]`
print(Array(outputData))
```

On return, the output descriptor contains a single value that is the square root of the sum of squares of each element in the tensor:

Specify an `axis_flags` of `0b100` to compute the norm along the second axis. In this case, the destination should be a matrix with a size that matches the zeroth and first dimensions of the source tensor:

```
let outputData = UnsafeMutableBufferPointer.allocate(capacity: 6)
var outputDescriptor = BNNSNDArrayDescriptor(flags: BNNSNDArrayFlags(0),
                                             layout: BNNSDataLayoutColumnMajorMatrix,
                                             size: (3, 2, 0, 0, 0, 0, 0, 0),
                                             stride: (0, 0, 0, 0, 0, 0, 0, 0),
                                             data: outputData.baseAddress!,
                                             data_type: BNNSDataType.float,
                                             table_data: nil,
                                             table_data_type: BNNSDataType.float,
                                             data_scale: 1, data_bias: 0)

BNNSComputeNorm(&outputDescriptor,
                 &inputDescriptor,
                 BNNSL2Norm,
                 0b100)

// Prints
//      [1005.0378, 2010.075, 3015.113,
//       4020.1511, 5025.189, 6030.227]
print(Array(outputData))
```

On return, the output descriptor contains six values that are the norms of the slices along the second axis of the input tensor:

To compute the norm along more that one dimension, define the destination tensor with a size of the dimensions you’re not calculating over. For example, the following code defines an `axis_flags` with a value of `0b101` to compute the norm of dimensions zero and two:

```
let outputData = UnsafeMutableBufferPointer.allocate(capacity: 2)
var outputDescriptor = BNNSNDArrayDescriptor(flags: BNNSNDArrayFlags(0),
                                             layout: BNNSDataLayoutVector,
                                             size: (2, 0, 0, 0, 0, 0, 0, 0),
                                             stride: (0, 0, 0, 0, 0, 0, 0, 0),
                                             data: outputData.baseAddress!,
                                             data_type: BNNSDataType.float,
                                             table_data: nil,
                                             table_data_type: BNNSDataType.float,
                                             data_scale: 1, data_bias: 0)

BNNSComputeNorm(&outputDescriptor,
                 &inputDescriptor,
                 BNNSL2Norm,
                 0b101)

// Prints `[3760.507, 8819.171]`
print(Array(outputData))
```

On return, the output descriptor contains two values that are the norms of the top and bottom slices of the input tensor:

## See Also

### Compute norm functions

static func computeNorm(input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, axes: [Int]?) throws

Computes the Euclidean norm and writes the result to the output tensor.

Deprecated

static func computeNormBackward(input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, axes: [Int]?, outputGradient: BNNSNDArrayDescriptor, generatingInputGradient: BNNSNDArrayDescriptor) throws

Backpropogates gradients for the compute norm function.

Deprecated

func BNNSComputeNormBackward(UnsafeRawPointer, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafeRawPointer, UnsafePointer&lt;BNNSNDArrayDescriptor>, BNNSNormType, UInt32) -> Int32

Backpropogates gradients for the compute norm function.

Deprecated

struct BNNSNormType

Constants that describe norm types.

