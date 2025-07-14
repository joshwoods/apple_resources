

- Accelerate
- BNNSArithmeticTernary
-  init(in1:in1_type:in2:in2_type:in3:in3_type:out:out_type:) Deprecated

Initializer

# init(in1:in1_type:in2:in2_type:in3:in3_type:out:out_type:)

Returns a new arithmetic structure that takes three inputs from the specified parameters.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
init(
    in1: BNNSNDArrayDescriptor,
    in1_type: BNNSDescriptorType,
    in2: BNNSNDArrayDescriptor,
    in2_type: BNNSDescriptorType,
    in3: BNNSNDArrayDescriptor,
    in3_type: BNNSDescriptorType,
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

`in3`  

The descriptor of the third input.

`in3_type`  

The descriptor type of the third input.

`out`  

The descriptor of the output.

`out_type`  

The descriptor type of the output.

## See Also

### Creating an Arithmetic Structure

init()

Returns a new arithmetic structure that takes three inputs.

Deprecated

