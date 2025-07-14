

- Accelerate
-  BNNSFilterApplyBackwardBatch(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:) Deprecated

Function

# BNNSFilterApplyBackwardBatch(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:)

Applies a filter backward to generate input delta, weights delta and bias delta.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
func BNNSFilterApplyBackwardBatch(
    _ filter: BNNSFilter?,
    _ batch_size: Int,
    _ in: UnsafeRawPointer?,
    _ in_stride: Int,
    _ in_delta: UnsafeMutablePointer?,
    _ in_delta_stride: Int,
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

`in`  

Pointer to input object.

`in_stride`  

Increment, in values, between input objects.

`in_delta`  

The descriptor of the input delta.

`in_delta_stride`  

Increment, in values, between input delta objects.

`out`  

Pointer to output object.

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

func BNNSFilterApplyBackwardTwoInputBatch(BNNSFilter?, Int, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, Int, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, Int, UnsafeRawPointer?, Int, UnsafePointer&lt;BNNSNDArrayDescriptor>, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?) -> Int32

Applies a filter backward to generate input deltas, weights delta and bias delta.

Deprecated

