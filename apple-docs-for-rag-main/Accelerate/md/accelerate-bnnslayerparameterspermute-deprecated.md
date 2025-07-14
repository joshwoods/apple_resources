

- Accelerate
-  BNNSLayerParametersPermute Deprecated

Structure

# BNNSLayerParametersPermute

A structure that contains the parameters of a permute layer.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
struct BNNSLayerParametersPermute
```

Deprecated

Use BNNSGraph\* APIs

## Topics

### Initializers

init(i_desc: BNNSNDArrayDescriptor, o_desc: BNNSNDArrayDescriptor, permutation: (Int, Int, Int, Int, Int, Int, Int, Int))

Returns a new permute layer parameters structure from the specified parameters.

init()

Returns a new permute layer parameters structure.

### Instance Properties

var i_desc: BNNSNDArrayDescriptor

The descriptor of the input.

var o_desc: BNNSNDArrayDescriptor

The descriptor of the output.

var permutation: (Int, Int, Int, Int, Int, Int, Int, Int)

The tuple that defines the permutation.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Permute layers

class PermuteLayer

A layer object that wraps a permute filter and manages its deinitialization.

Deprecated

func BNNSFilterCreateLayerPermute(UnsafePointer&lt;BNNSLayerParametersPermute>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new permute layer.

Deprecated

func BNNSPermuteFilterApplyBackwardBatch(BNNSFilter?, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, Int, UnsafePointer&lt;BNNSNDArrayDescriptor>, Int) -> Int32

Applies a permute filter backward to generate gradients.

Deprecated

