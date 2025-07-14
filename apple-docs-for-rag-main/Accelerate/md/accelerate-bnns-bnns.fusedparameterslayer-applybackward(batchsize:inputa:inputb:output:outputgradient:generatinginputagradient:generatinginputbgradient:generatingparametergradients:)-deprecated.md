

- Accelerate
- BNNS
- BNNS.FusedParametersLayer
-  applyBackward(batchSize:inputA:inputB:output:outputGradient:generatingInputAGradient:generatingInputBGradient:generatingParameterGradients:) Deprecated

Instance Method

# applyBackward(batchSize:inputA:inputB:output:outputGradient:generatingInputAGradient:generatingInputBGradient:generatingParameterGradients:)

Applies the layer backward to generate input gradients, where the first layer accepts two inputs.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
func applyBackward(
    batchSize: Int,
    inputA: BNNSNDArrayDescriptor,
    inputB: BNNSNDArrayDescriptor,
    output: BNNSNDArrayDescriptor,
    outputGradient: BNNSNDArrayDescriptor,
    generatingInputAGradient inputAGradient: BNNSNDArrayDescriptor,
    generatingInputBGradient inputBGradient: BNNSNDArrayDescriptor,
    generatingParameterGradients parameterGradients: [BNNSNDArrayDescriptor]
) throws
```

Deprecated

Use the BNNSGraph API instead.

## Parameters 

`batchSize`  

The number of input-output pairs.

`inputA`  

The descriptor of the first input.

`inputB`  

The descriptor of the second input.

`output`  

The descriptor of the output.

`outputGradient`  

The descriptor of the output gradient.

`inputAGradient`  

The descriptor of the input gradient.

`inputBGradient`  

The descriptor of the input gradient.

`parameterGradients`  

An array that contains the parameter gradients.

## See Also

### Applying a Fused Parameters Layer

func apply(batchSize: Int, inputA: BNNSNDArrayDescriptor, inputB: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, for: BNNS.LearningPhase) throws

Applies the layer to a set of input objects and writes the result to a set of output objects, where the first layer accepts two inputs.

Deprecated

func apply(batchSize: Int, inputA: BNNSNDArrayDescriptor, inputB: BNNSNDArrayDescriptor, inputC: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, for: BNNS.LearningPhase) throws

Applies the layer to a set of input objects and writes the result to a set of output objects, where the first layer accepts two inputs.

Deprecated

func applyBackward(batchSize: Int, inputA: BNNSNDArrayDescriptor, inputB: BNNSNDArrayDescriptor, inputC: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, outputGradient: BNNSNDArrayDescriptor, generatingInputAGradient: BNNSNDArrayDescriptor, generatingInputBGradient: BNNSNDArrayDescriptor, generatingInputCGradient: BNNSNDArrayDescriptor, generatingParameterGradients: [BNNSNDArrayDescriptor]) throws

Applies the layer backward to generate input gradients, where the first layer accepts three inputs.

Deprecated

