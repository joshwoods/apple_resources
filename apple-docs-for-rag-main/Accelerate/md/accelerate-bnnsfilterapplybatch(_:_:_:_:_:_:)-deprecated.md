

- Accelerate
-  BNNSFilterApplyBatch(\_:\_:\_:\_:\_:\_:) Deprecated

Function

# BNNSFilterApplyBatch(\_:\_:\_:\_:\_:\_:)

Applies a filter to a set of input objects, writing the result to a set of output objects.

iOS 10.0–18.0DeprecatediPadOS 10.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.12–15.0DeprecatedtvOS 10.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 3.0–11.0Deprecated

``` source
func BNNSFilterApplyBatch(
    _ filter: BNNSFilter?,
    _ batch_size: Int,
    _ in: UnsafeRawPointer,
    _ in_stride: Int,
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

`in`  

Pointer to input object.

`in_stride`  

Increment, in values, between input objects.

`out`  

Pointer to output object.

`out_stride`  

Increment, in values, between output objects.

## Return Value

## See Also

### Forward Propagation Functions

func BNNSFilterApply(BNNSFilter?, UnsafeRawPointer, UnsafeMutableRawPointer) -> Int32

Applies a filter to an input, writing the result to a specified output.

Deprecated

func BNNSFilterApplyTwoInput(BNNSFilter?, UnsafeRawPointer, UnsafeRawPointer, UnsafeMutableRawPointer) -> Int32

Applies a filter to a pair of inputs, writing the result to a specified output.

Deprecated

func BNNSFilterApplyTwoInputBatch(BNNSFilter?, Int, UnsafeRawPointer, Int, UnsafeRawPointer, Int, UnsafeMutableRawPointer, Int) -> Int32

Applies a filter to a set of input object pairs, writing the result to a set of output objects.

Deprecated

