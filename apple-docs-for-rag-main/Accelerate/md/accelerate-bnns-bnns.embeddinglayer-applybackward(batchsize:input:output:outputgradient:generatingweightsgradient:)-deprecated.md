

- Accelerate
- BNNS
- BNNS.EmbeddingLayer
-  applyBackward(batchSize:input:output:outputGradient:generatingWeightsGradient:) Deprecated

Instance Method

# applyBackward(batchSize:input:output:outputGradient:generatingWeightsGradient:)

Applies the layer backward to generate input gradients.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
func applyBackward(
    batchSize: Int,
    input: BNNSNDArrayDescriptor,
    output: BNNSNDArrayDescriptor,
    outputGradient: BNNSNDArrayDescriptor,
    generatingWeightsGradient weightsGradient: BNNSNDArrayDescriptor
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

`weightsGradient`  

The descriptor of the input gradient.

## See Also

### Applying an Embedding Layer

func apply(batchSize: Int, input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor) throws

Applies the layer to a set of input objects, writing the result to a set of output objects.

Deprecated

