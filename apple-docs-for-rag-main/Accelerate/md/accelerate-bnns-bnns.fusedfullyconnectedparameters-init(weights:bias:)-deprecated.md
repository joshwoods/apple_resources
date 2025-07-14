

- Accelerate
- BNNS
- BNNS.FusedFullyConnectedParameters
-  init(weights:bias:) Deprecated

Initializer

# init(weights:bias:)

Returns a new fused dequantization parameters structure.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+Mac Catalyst

``` source
init(
    weights: BNNSNDArrayDescriptor,
    bias: BNNSNDArrayDescriptor?
)
```

Deprecated

Use the BNNSGraph API instead.

## Parameters 

`weights`  

The descriptor of the weights.

`bias`  

The descriptor of the bias.

