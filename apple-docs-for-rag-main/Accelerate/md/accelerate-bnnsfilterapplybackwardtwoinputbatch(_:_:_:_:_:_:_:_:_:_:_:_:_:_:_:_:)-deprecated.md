

- Accelerate
-  BNNSFilterApplyBackwardTwoInputBatch(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:) Deprecated

Function

# BNNSFilterApplyBackwardTwoInputBatch(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:)

Applies a filter backward to generate input deltas, weights delta and bias delta.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
func BNNSFilterApplyBackwardTwoInputBatch(
    _ filter: BNNSFilter?,
    _ batch_size: Int,
    _ inA: UnsafeRawPointer?,
    _ inA_stride: Int,
    _ inA_delta: UnsafeMutablePointer?,
    _ inA_delta_stride: Int,
    _ inB: UnsafeRawPointer?,
    _ inB_stride: Int,
    _ inB_delta: UnsafeMutablePointer?,
    _ inB_delta_stride: Int,
    _ out: UnsafeRawPointer?,
    _ out_stride: Int,
    _ out_delta: UnsafePointer,
    _ out_delta_stride: Int,
    _ weights_delta: UnsafeMutablePointer?,
    _ bias_delta: UnsafeMutablePointer?
) -> Int32
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`filter`  

The filter to apply.

`batch_size`  

The number of input-output pairs.

`inA`  

Pointer to the first input data.

`inA_stride`  

Increment, in values, between first input objects.

`inA_delta`  

The descriptor of the first input delta.

`inA_delta_stride`  

Increment, in values, between first input delta objects.

`inB`  

Pointer to the second input data.

`inB_stride`  

Increment, in values, between second input objects.

`inB_delta`  

The descriptor of the second input delta.

`inB_delta_stride`  

Increment, in values, between second input delta objects.

`out`  

Pointer to the output data.

`out_stride`  

Increment, in values, between output objects.

`out_delta`  

The descriptor of the output delta.

`out_delta_stride`  

Increment, in values, between output delta objects.

`weights_delta`  

The descriptor of the weights delta.

`bias_delta`  

The descriptor of the bias delta.

## See Also

### Backpropagation Functions

func BNNSFilterApplyBackwardBatch(BNNSFilter?, Int, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, Int, UnsafeRawPointer?, Int, UnsafePointer&lt;BNNSNDArrayDescriptor>, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?) -> Int32

Applies a filter backward to generate input delta, weights delta and bias delta.

Deprecated

