

- Accelerate
- BNNS
- BNNS.LossLayer
-  apply(batchSize:input:labels:output:weights:broadcastsWeights:generatingInputGradient:) Deprecated

Instance Method

# apply(batchSize:input:labels:output:weights:broadcastsWeights:generatingInputGradient:)

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+visionOSwatchOS 8.0+tvOS 15.0+

``` source
func apply(
    batchSize: Int,
    input: BNNSNDArrayDescriptor,
    labels: BNNSNDArrayDescriptor,
    output: BNNSNDArrayDescriptor,
    weights: BNNSNDArrayDescriptor?,
    broadcastsWeights: Bool,
    generatingInputGradient inputGradient: BNNSNDArrayDescriptor
) throws
```

Deprecated

Use the BNNSGraph API instead.

