

- Accelerate
-  BNNSFilterApplyTwoInputBatch(\_:\_:\_:\_:\_:\_:\_:\_:) Deprecated

Function

# BNNSFilterApplyTwoInputBatch(\_:\_:\_:\_:\_:\_:\_:\_:)

Applies a filter to a set of input object pairs, writing the result to a set of output objects.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
func BNNSFilterApplyTwoInputBatch(
    _ filter: BNNSFilter?,
    _ batch_size: Int,
    _ inA: UnsafeRawPointer,
    _ inA_stride: Int,
    _ inB: UnsafeRawPointer,
    _ inB_stride: Int,
    _ out: UnsafeMutableRawPointer,
    _ out_stride: Int
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

`inB`  

Pointer to the second input data.

`inB_stride`  

Increment, in values, between second input objects.

`out`  

Pointer to the output data.

`out_stride`  

Increment, in values, between output objects.

## See Also

### Forward Propagation Functions

func BNNSFilterApply(BNNSFilter?, UnsafeRawPointer, UnsafeMutableRawPointer) -> Int32

Applies a filter to an input, writing the result to a specified output.

Deprecated

func BNNSFilterApplyBatch(BNNSFilter?, Int, UnsafeRawPointer, Int, UnsafeMutableRawPointer, Int) -> Int32

Applies a filter to a set of input objects, writing the result to a set of output objects.

Deprecated

func BNNSFilterApplyTwoInput(BNNSFilter?, UnsafeRawPointer, UnsafeRawPointer, UnsafeMutableRawPointer) -> Int32

Applies a filter to a pair of inputs, writing the result to a specified output.

Deprecated

