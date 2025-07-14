

- Accelerate
- BNNS
- BNNS.FusedLayer
-  applyBackward(batchSize:input:output:outputGradient:generatingInputGradient:generatingParameterGradients:) Deprecated

Instance Method

# applyBackward(batchSize:input:output:outputGradient:generatingInputGradient:generatingParameterGradients:)

Applies the layer backward to generate input gradients.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+visionOSwatchOS 7.0+tvOS 14.0+

``` source
func applyBackward(
    batchSize: Int,
    input: BNNSNDArrayDescriptor,
    output: BNNSNDArrayDescriptor,
    outputGradient: BNNSNDArrayDescriptor,
    generatingInputGradient inputGradient: BNNSNDArrayDescriptor,
    generatingParameterGradients parameterGradients: [BNNSNDArrayDescriptor]
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

`parameterGradients`  

An array that contains the parameter gradients.

## See Also

### Applying a Fused Layer

func apply(batchSize: Int, input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, for: BNNS.LearningPhase) throws

Applies the layer to a set of input objects, writing the result to a set of output objects.

Deprecated

