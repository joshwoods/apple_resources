

- Accelerate
- BNNS
- BNNS.NormalizationLayer
-  apply(batchSize:input:output:for:) Deprecated

Instance Method

# apply(batchSize:input:output:for:)

Applies the layer to a set of input objects, writing the result to a set of output objects.

iOS 14.0+iPadOS 14.0+macOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+Mac Catalyst

``` source
func apply(
    batchSize: Int,
    input: BNNSNDArrayDescriptor,
    output: BNNSNDArrayDescriptor,
    for learningPhase: BNNS.LearningPhase
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

`learningPhase`  

An enumeration that specifies whether the function call context is training or inference.

## See Also

### Applying a Normalization Layer

func applyBackward(batchSize: Int, input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, outputGradient: BNNSNDArrayDescriptor, generatingInputGradient: BNNSNDArrayDescriptor, generatingBetaGradient: BNNSNDArrayDescriptor?, generatingGammaGradient: BNNSNDArrayDescriptor?) throws

Applies the layer backward to generate input gradients.

Deprecated

