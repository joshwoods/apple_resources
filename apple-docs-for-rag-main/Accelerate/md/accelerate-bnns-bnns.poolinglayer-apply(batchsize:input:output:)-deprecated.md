

- Accelerate
- BNNS
- BNNS.PoolingLayer
-  apply(batchSize:input:output:) Deprecated

Instance Method

# apply(batchSize:input:output:)

Applies the layer to a set of input objects, writing the result to a set of output objects.

iOS 14.0+iPadOS 14.0+macOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+Mac Catalyst

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

### Applying a Pooling Layer

func applyBackward(batchSize: Int, input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, outputGradient: BNNSNDArrayDescriptor, generatingInputGradient: BNNSNDArrayDescriptor, generatingBiasGradient: BNNSNDArrayDescriptor?) throws

Applies the layer backward to generate input gradients.

Deprecated

