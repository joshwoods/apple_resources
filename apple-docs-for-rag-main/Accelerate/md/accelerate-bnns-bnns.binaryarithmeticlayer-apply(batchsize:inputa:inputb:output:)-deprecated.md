

- Accelerate
- BNNS
- BNNS.BinaryArithmeticLayer
-  apply(batchSize:inputA:inputB:output:) Deprecated

Instance Method

# apply(batchSize:inputA:inputB:output:)

Applies the layer to a set of input array descriptors, writing the result to a set of output array descriptors.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
func apply(
    batchSize: Int,
    inputA: BNNSNDArrayDescriptor,
    inputB: BNNSNDArrayDescriptor,
    output: BNNSNDArrayDescriptor
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

## See Also

### Applying a Binary Arithmetic Layer

func applyBackward(batchSize: Int, inputA: BNNSNDArrayDescriptor, inputB: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, outputGradient: BNNSNDArrayDescriptor, generatingInputAGradient: BNNSNDArrayDescriptor, generatingInputBGradient: BNNSNDArrayDescriptor) throws

Applies the layer backward to generate input gradients.

Deprecated

