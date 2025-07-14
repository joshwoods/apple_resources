

- Accelerate
- BNNS
-  BNNS.PermuteLayer Deprecated

Class

# BNNS.PermuteLayer

A layer object that wraps a permute filter and manages its deinitialization.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
class PermuteLayer
```

Deprecated

Use the BNNSGraph API instead.

## Topics

### Creating a Permute Layer

convenience init?(input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, permutation: [Int], filterParameters: BNNSFilterParameters?)

Returns a new permute layer.

## Relationships

### Inherits From

- BNNS.UnaryLayer

## See Also

### Permute layers

struct BNNSLayerParametersPermute

A structure that contains the parameters of a permute layer.

Deprecated

func BNNSFilterCreateLayerPermute(UnsafePointer&lt;BNNSLayerParametersPermute>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new permute layer.

Deprecated

func BNNSPermuteFilterApplyBackwardBatch(BNNSFilter?, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, Int, UnsafePointer&lt;BNNSNDArrayDescriptor>, Int) -> Int32

Applies a permute filter backward to generate gradients.

Deprecated

