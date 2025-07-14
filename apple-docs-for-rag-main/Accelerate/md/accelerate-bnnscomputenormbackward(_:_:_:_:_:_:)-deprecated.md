

- Accelerate
-  BNNSComputeNormBackward(\_:\_:\_:\_:\_:\_:) Deprecated

Function

# BNNSComputeNormBackward(\_:\_:\_:\_:\_:\_:)

Backpropogates gradients for the compute norm function.

iOS 15.0–18.0DeprecatediPadOS 15.0–18.0DeprecatedMac Catalyst 15.0–18.0DeprecatedmacOS 12.0–15.0DeprecatedtvOS 15.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 8.0–11.0Deprecated

``` source
func BNNSComputeNormBackward(
    _ in: UnsafeRawPointer,
    _ in_delta: UnsafeMutablePointer,
    _ out: UnsafeRawPointer,
    _ out_delta: UnsafePointer,
    _ norm_type: BNNSNormType,
    _ axis_flags: UInt32
) -> Int32
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`in`  

The descriptor of the input.

`in_delta`  

The descriptor of the input delta.

`out`  

The descriptor of the output.

`out_delta`  

The descriptor of the output delta.

`norm_type`  

The type of the norm. This function supports only BNNSL2Norm.

`axis_flags`  

The dimensions that the function uses to compute the norm. Set to `0` to specify that the function computes the norm over all dimensions.

## See Also

### Compute norm functions

static func computeNorm(input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, axes: [Int]?) throws

Computes the Euclidean norm and writes the result to the output tensor.

Deprecated

static func computeNormBackward(input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, axes: [Int]?, outputGradient: BNNSNDArrayDescriptor, generatingInputGradient: BNNSNDArrayDescriptor) throws

Backpropogates gradients for the compute norm function.

Deprecated

func BNNSComputeNorm(UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, BNNSNormType, UInt32) -> Int32

Computes the specified norm over an entire tensor or the specified axes.

Deprecated

struct BNNSNormType

Constants that describe norm types.

