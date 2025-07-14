

- Accelerate
- BNNSLayerParametersPermute
-  init(i_desc:o_desc:permutation:) Deprecated

Initializer

# init(i_desc:o_desc:permutation:)

Returns a new permute layer parameters structure from the specified parameters.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
init(
    i_desc: BNNSNDArrayDescriptor,
    o_desc: BNNSNDArrayDescriptor,
    permutation: (Int, Int, Int, Int, Int, Int, Int, Int)
)
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`i_desc`  

The descriptor of the input.

`o_desc`  

The descriptor of the output.

`permutation`  

The tuple that defines the permutation.

## Discussion

Use the permutation array to specify the input axis source for the corresponding output axis source. For example, a permutation array \[2,1,0\] applied on a BNNSDataLayoutImageCHW tensor results in axis reverse (that is, output axis 0 is input axis 2, output axis 1 is input axis 1, and output axis 2 is input axis 0).

Important

The number of input dimensions must be equal to number of output dimensions.

## See Also

### Initializers

init()

Returns a new permute layer parameters structure.

Deprecated

