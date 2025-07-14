

- Accelerate
- BNNSArithmeticBinary
-  init(in1:in1_type:in2:in2_type:out:out_type:) Deprecated

Initializer

# init(in1:in1_type:in2:in2_type:out:out_type:)

Returns a new arithmetic structure that takes two inputs from the specified parameters.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
init(
    in1: BNNSNDArrayDescriptor,
    in1_type: BNNSDescriptorType,
    in2: BNNSNDArrayDescriptor,
    in2_type: BNNSDescriptorType,
    out: BNNSNDArrayDescriptor,
    out_type: BNNSDescriptorType
)
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`in1`  

The descriptor of the first input.

`in1_type`  

The descriptor type of the first input.

`in2`  

The descriptor of the second input.

`in2_type`  

The descriptor type of the second input.

`out`  

The descriptor of the output.

`out_type`  

The descriptor type of the output.

## Discussion

Important

The data types of the inputs must be equal to the output data type. The size of the inputs must either 1, or the maximum size of either input and the output. Arithmetic layers only support arrays with a data type of `float`, and a data layout of BNNS.DataLayout.vector, BNNS.DataLayout.matrixRowMajor, BNNS.DataLayout.matrixColumnMajor, or BNNS.DataLayout.imageCHW.

## See Also

### Creating an Arithmetic Structure

init()

Returns a new arithmetic structure that takes two inputs.

Deprecated

