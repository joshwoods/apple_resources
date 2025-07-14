

- Accelerate
-  BNNSFilterApply(\_:\_:\_:) Deprecated

Function

# BNNSFilterApply(\_:\_:\_:)

Applies a filter to an input, writing the result to a specified output.

iOS 10.0–18.0DeprecatediPadOS 10.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.12–15.0DeprecatedtvOS 10.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 3.0–11.0Deprecated

``` source
func BNNSFilterApply(
    _ filter: BNNSFilter?,
    _ in: UnsafeRawPointer,
    _ out: UnsafeMutableRawPointer
) -> Int32
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`filter`  

The filter to apply.

`in`  

Pointer to the input data.

`out`  

Pointer to the output data.

## Return Value

Returns 0 on success, -1 on failure.

## See Also

### Forward Propagation Functions

func BNNSFilterApplyBatch(BNNSFilter?, Int, UnsafeRawPointer, Int, UnsafeMutableRawPointer, Int) -> Int32

Applies a filter to a set of input objects, writing the result to a set of output objects.

Deprecated

func BNNSFilterApplyTwoInput(BNNSFilter?, UnsafeRawPointer, UnsafeRawPointer, UnsafeMutableRawPointer) -> Int32

Applies a filter to a pair of inputs, writing the result to a specified output.

Deprecated

func BNNSFilterApplyTwoInputBatch(BNNSFilter?, Int, UnsafeRawPointer, Int, UnsafeRawPointer, Int, UnsafeMutableRawPointer, Int) -> Int32

Applies a filter to a set of input object pairs, writing the result to a set of output objects.

Deprecated

