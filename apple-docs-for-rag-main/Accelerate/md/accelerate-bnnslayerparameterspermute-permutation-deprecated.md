

- Accelerate
- BNNSLayerParametersPermute
-  permutation Deprecated

Instance Property

# permutation

The tuple that defines the permutation.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
var permutation: (Int, Int, Int, Int, Int, Int, Int, Int)
```

Deprecated

Use BNNSGraph\* APIs

## Discussion

Use the permutation array to specify the input axis source for the corresponding output axis source. For example, a permutation array \[2,1,0\] applied on a BNNSDataLayoutImageCHW tensor results in axis reverse (that is, output axis 0 is input axis 2, output axis 1 is input axis 1, and output axis 2 is input axis 0).

## See Also

### Instance Properties

var i_desc: BNNSNDArrayDescriptor

The descriptor of the input.

Deprecated

var o_desc: BNNSNDArrayDescriptor

The descriptor of the output.

Deprecated

