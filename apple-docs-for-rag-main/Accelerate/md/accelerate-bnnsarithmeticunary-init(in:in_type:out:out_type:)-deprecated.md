

- Accelerate
- BNNSArithmeticUnary
-  init(in:in_type:out:out_type:) Deprecated

Initializer

# init(in:in_type:out:out_type:)

Returns a new arithmetic structure that takes a single input from the specified parameters.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
init(
    in: BNNSNDArrayDescriptor,
    in_type: BNNSDescriptorType,
    out: BNNSNDArrayDescriptor,
    out_type: BNNSDescriptorType
)
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`in`  

The descriptor of the input.

`in_type`  

The descriptor type of the input.

`out`  

The descriptor of the output.

`out_type`  

The descriptor type of the output.

## Discussion

Important

The input data type must be equal to the output data type. The input size must equal the output size or `1`. Arithmetic layers only support arrays with a data type of `float`, and a data layout of BNNS.DataLayout.vector, BNNS.DataLayout.matrixRowMajor, BNNS.DataLayout.matrixColumnMajor, or BNNS.DataLayout.imageCHW.

## See Also

### Creating an Arithmetic Structure

init()

Returns a new arithmetic structure that takes a single input.

Deprecated

