

- Accelerate
- BNNS
- BNNS.BinaryArithmeticLayer
-  applyBackward(batchSize:inputA:inputB:output:outputGradient:generatingInputAGradient:generatingInputBGradient:) Deprecated

Instance Method

# applyBackward(batchSize:inputA:inputB:output:outputGradient:generatingInputAGradient:generatingInputBGradient:)

Applies the layer backward to generate input gradients.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+watchOS 7.0+visionOS

``` source
func applyBackward(
    batchSize: Int,
    inputA: BNNSNDArrayDescriptor,
    inputB: BNNSNDArrayDescriptor,
    output: BNNSNDArrayDescriptor,
    outputGradient: BNNSNDArrayDescriptor,
    generatingInputAGradient inputAGradient: BNNSNDArrayDescriptor,
    generatingInputBGradient inputBGradient: BNNSNDArrayDescriptor
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

The descriptor of the first input gradient.

`inputBGradient`  

The descriptor of the second input gradient.

## See Also

### Applying a Binary Arithmetic Layer

func apply(batchSize: Int, inputA: BNNSNDArrayDescriptor, inputB: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor) throws

Applies the layer to a set of input array descriptors, writing the result to a set of output array descriptors.

Deprecated

