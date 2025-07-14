

- Accelerate
-  BNNSFilterApplyTwoInput(\_:\_:\_:\_:) Deprecated

Function

# BNNSFilterApplyTwoInput(\_:\_:\_:\_:)

Applies a filter to a pair of inputs, writing the result to a specified output.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
func BNNSFilterApplyTwoInput(
    _ filter: BNNSFilter?,
    _ inA: UnsafeRawPointer,
    _ inB: UnsafeRawPointer,
    _ out: UnsafeMutableRawPointer
) -> Int32
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`filter`  

The filter to apply.

`inA`  

Pointer to the first input data.

`inB`  

Pointer to the second input data.

`out`  

Pointer to the output data.

## See Also

### Forward Propagation Functions

func BNNSFilterApply(BNNSFilter?, UnsafeRawPointer, UnsafeMutableRawPointer) -> Int32

Applies a filter to an input, writing the result to a specified output.

Deprecated

func BNNSFilterApplyBatch(BNNSFilter?, Int, UnsafeRawPointer, Int, UnsafeMutableRawPointer, Int) -> Int32

Applies a filter to a set of input objects, writing the result to a set of output objects.

Deprecated

func BNNSFilterApplyTwoInputBatch(BNNSFilter?, Int, UnsafeRawPointer, Int, UnsafeRawPointer, Int, UnsafeMutableRawPointer, Int) -> Int32

Applies a filter to a set of input object pairs, writing the result to a set of output objects.

Deprecated

