

- Accelerate
- BNNS
- BNNS.EmbeddingLayer
-  apply(batchSize:input:output:) Deprecated

Instance Method

# apply(batchSize:input:output:)

Applies the layer to a set of input objects, writing the result to a set of output objects.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
func apply(
    batchSize: Int,
    input: BNNSNDArrayDescriptor,
    output: BNNSNDArrayDescriptor
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

## See Also

### Applying an Embedding Layer

func applyBackward(batchSize: Int, input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, outputGradient: BNNSNDArrayDescriptor, generatingWeightsGradient: BNNSNDArrayDescriptor) throws

Applies the layer backward to generate input gradients.

Deprecated

