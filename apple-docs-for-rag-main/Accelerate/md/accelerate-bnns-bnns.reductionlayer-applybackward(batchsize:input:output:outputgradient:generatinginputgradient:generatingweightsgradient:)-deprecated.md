

- Accelerate
- BNNS
- BNNS.ReductionLayer
-  applyBackward(batchSize:input:output:outputGradient:generatingInputGradient:generatingWeightsGradient:) Deprecated

Instance Method

# applyBackward(batchSize:input:output:outputGradient:generatingInputGradient:generatingWeightsGradient:)

Applies the layer backward to generate input gradients.

iOS 14.0+iPadOS 14.0+macOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+Mac Catalyst

``` source
func applyBackward(
    batchSize: Int,
    input: BNNSNDArrayDescriptor,
    output: BNNSNDArrayDescriptor,
    outputGradient: BNNSNDArrayDescriptor,
    generatingInputGradient inputGradient: BNNSNDArrayDescriptor,
    generatingWeightsGradient weightsGradient: BNNSNDArrayDescriptor? = nil
) throws
```

Deprecated

Use the BNNSGraph API instead.

## Parameters 

`batchSize`  

The number of input-output pairs.

`input`  

The descriptor of the input.

`output`  

The descriptor of the output.

`outputGradient`  

The descriptor of the output gradient.

`inputGradient`  

The descriptor of the input gradient.

`weightsGradient`  

The descriptor of the weights gradient.

