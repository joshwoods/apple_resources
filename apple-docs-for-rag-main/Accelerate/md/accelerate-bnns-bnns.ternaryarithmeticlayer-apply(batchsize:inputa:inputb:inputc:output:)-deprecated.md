

- Accelerate
- BNNS
- BNNS.TernaryArithmeticLayer
-  apply(batchSize:inputA:inputB:inputC:output:) Deprecated

Instance Method

# apply(batchSize:inputA:inputB:inputC:output:)

Applies the layer to a set of input array descriptors, writing the result to a set of output array descriptors.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+watchOS 8.0+visionOS

``` source
func apply(
    batchSize: Int,
    inputA: BNNSNDArrayDescriptor,
    inputB: BNNSNDArrayDescriptor,
    inputC: BNNSNDArrayDescriptor,
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

`inputC`  

The descriptor of the third input.

`output`  

The descriptor of the output.

## See Also

### Applying a Ternary Arithmetic Layer

func applyBackward(batchSize: Int, inputA: BNNSNDArrayDescriptor, inputB: BNNSNDArrayDescriptor, inputC: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, outputGradient: BNNSNDArrayDescriptor, generatingInputAGradient: BNNSNDArrayDescriptor, generatingInputBGradient: BNNSNDArrayDescriptor, generatingInputCGradient: BNNSNDArrayDescriptor) throws

Applies the layer backward to generate input gradients.

Deprecated

