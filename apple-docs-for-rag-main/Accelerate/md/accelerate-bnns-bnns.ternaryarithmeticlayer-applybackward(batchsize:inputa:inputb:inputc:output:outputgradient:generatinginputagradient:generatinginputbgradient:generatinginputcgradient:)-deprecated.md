

- Accelerate
- BNNS
- BNNS.TernaryArithmeticLayer
-  applyBackward(batchSize:inputA:inputB:inputC:output:outputGradient:generatingInputAGradient:generatingInputBGradient:generatingInputCGradient:) Deprecated

Instance Method

# applyBackward(batchSize:inputA:inputB:inputC:output:outputGradient:generatingInputAGradient:generatingInputBGradient:generatingInputCGradient:)

Applies the layer backward to generate input gradients.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
func applyBackward(
    batchSize: Int,
    inputA: BNNSNDArrayDescriptor,
    inputB: BNNSNDArrayDescriptor,
    inputC: BNNSNDArrayDescriptor,
    output: BNNSNDArrayDescriptor,
    outputGradient: BNNSNDArrayDescriptor,
    generatingInputAGradient inputAGradient: BNNSNDArrayDescriptor,
    generatingInputBGradient inputBGradient: BNNSNDArrayDescriptor,
    generatingInputCGradient inputCGradient: BNNSNDArrayDescriptor
) throws
```

Deprecated

Use the BNNSGraph API instead.

## Parameters 

`batchSize`  

The number of input-output pairs.

`inputA`  

The descriptor of the first input..

`inputB`  

The descriptor of the second input.

`inputC`  

The descriptor of the third input.

`output`  

The descriptor of the output.

`outputGradient`  

The descriptor of the output gradient.

`inputAGradient`  

The descriptor of the first input gradient.

`inputBGradient`  

The descriptor of the second input gradient.

`inputCGradient`  

The descriptor of the third input gradient.

## See Also

### Applying a Ternary Arithmetic Layer

func apply(batchSize: Int, inputA: BNNSNDArrayDescriptor, inputB: BNNSNDArrayDescriptor, inputC: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor) throws

Applies the layer to a set of input array descriptors, writing the result to a set of output array descriptors.

Deprecated

