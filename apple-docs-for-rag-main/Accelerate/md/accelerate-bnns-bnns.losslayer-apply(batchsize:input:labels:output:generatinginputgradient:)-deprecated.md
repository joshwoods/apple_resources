

- Accelerate
- BNNS
- BNNS.LossLayer
-  apply(batchSize:input:labels:output:generatingInputGradient:) Deprecated

Instance Method

# apply(batchSize:input:labels:output:generatingInputGradient:)

Applies the layer to a set of input objects, writing the result to a set of output objects.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
func apply(
    batchSize: Int,
    input: BNNSNDArrayDescriptor,
    labels: BNNSNDArrayDescriptor,
    output: BNNSNDArrayDescriptor,
    generatingInputGradient inputGradient: BNNSNDArrayDescriptor
) throws
```

Deprecated

Use the BNNSGraph API instead.

## Parameters 

`batchSize`  

The number of input-output pairs.

`input`  

The descriptor of the input.

`labels`  

The descriptor of the labels.

`output`  

The descriptor of the output.

`inputGradient`  

The descriptor of the input gradient.

