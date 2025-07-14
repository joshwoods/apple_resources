

- Accelerate
- BNNS
- BNNS.ConvolutionLayer
-  applyBackward(batchSize:input:output:outputGradient:generatingInputGradient:generatingWeightsGradient:generatingBiasGradient:) Deprecated

Instance Method

# applyBackward(batchSize:input:output:outputGradient:generatingInputGradient:generatingWeightsGradient:generatingBiasGradient:)

Applies the layer backward to generate input gradients.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+visionOSwatchOS 7.0+tvOS 14.0+

``` source
func applyBackward(
    batchSize: Int,
    input: BNNSNDArrayDescriptor,
    output: BNNSNDArrayDescriptor,
    outputGradient: BNNSNDArrayDescriptor,
    generatingInputGradient inputGradient: BNNSNDArrayDescriptor,
    generatingWeightsGradient weightsGradient: BNNSNDArrayDescriptor? = nil,
    generatingBiasGradient biasGradient: BNNSNDArrayDescriptor? = nil
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

`biasGradient`  

The descriptor of the bias gradient.

