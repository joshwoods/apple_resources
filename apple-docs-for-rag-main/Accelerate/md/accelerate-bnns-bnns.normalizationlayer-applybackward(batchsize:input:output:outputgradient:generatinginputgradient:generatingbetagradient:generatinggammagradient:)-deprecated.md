

- Accelerate
- BNNS
- BNNS.NormalizationLayer
-  applyBackward(batchSize:input:output:outputGradient:generatingInputGradient:generatingBetaGradient:generatingGammaGradient:) Deprecated

Instance Method

# applyBackward(batchSize:input:output:outputGradient:generatingInputGradient:generatingBetaGradient:generatingGammaGradient:)

Applies the layer backward to generate input gradients.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
func applyBackward(
    batchSize: Int,
    input: BNNSNDArrayDescriptor,
    output: BNNSNDArrayDescriptor,
    outputGradient: BNNSNDArrayDescriptor,
    generatingInputGradient inputGradient: BNNSNDArrayDescriptor,
    generatingBetaGradient betaGradient: BNNSNDArrayDescriptor? = nil,
    generatingGammaGradient gammaGradient: BNNSNDArrayDescriptor? = nil
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

`betaGradient`  

The descriptor of the beta gradient.

`gammaGradient`  

The descriptor of the gamma gradient.

## See Also

### Applying a Normalization Layer

func apply(batchSize: Int, input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, for: BNNS.LearningPhase) throws

Applies the layer to a set of input objects, writing the result to a set of output objects.

Deprecated

