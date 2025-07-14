

- Accelerate
- BNNS
- BNNS.BroadcastMatrixMultiplyLayer
-  applyBackward(batchSize:inputA:inputB:output:outputGradient:generatingInputAGradient:generatingInputBGradient:) Deprecated

Instance Method

# applyBackward(batchSize:inputA:inputB:output:outputGradient:generatingInputAGradient:generatingInputBGradient:)

Applies the layer backward to generate input gradients.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

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

The descriptor of matrix *A*.

`inputB`  

The descriptor of matrix *B*.

`output`  

The descriptor of the output.

`outputGradient`  

The descriptor of the output gradient.

`inputAGradient`  

The descriptor of the matrix *A* gradient.

`inputBGradient`  

The descriptor of the matrix *B* gradient.

