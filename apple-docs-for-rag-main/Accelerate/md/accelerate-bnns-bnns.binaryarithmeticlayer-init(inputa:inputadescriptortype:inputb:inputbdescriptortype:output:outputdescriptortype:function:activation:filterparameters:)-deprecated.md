

- Accelerate
- BNNS
- BNNS.BinaryArithmeticLayer
-  init(inputA:inputADescriptorType:inputB:inputBDescriptorType:output:outputDescriptorType:function:activation:filterParameters:) Deprecated

Initializer

# init(inputA:inputADescriptorType:inputB:inputBDescriptorType:output:outputDescriptorType:function:activation:filterParameters:)

Returns a new binary arithmetic layer.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
convenience init?(
    inputA: BNNSNDArrayDescriptor,
    inputADescriptorType: BNNS.DescriptorType,
    inputB: BNNSNDArrayDescriptor,
    inputBDescriptorType: BNNS.DescriptorType,
    output: BNNSNDArrayDescriptor,
    outputDescriptorType: BNNS.DescriptorType,
    function: BNNS.ArithmeticBinaryFunction,
    activation: BNNS.ActivationFunction = .identity,
    filterParameters: BNNSFilterParameters? = nil
)
```

Deprecated

Use the BNNSGraph API instead.

## Parameters 

`inputA`  

The descriptor of the first input.

`inputADescriptorType`  

The descriptor type of the first input.

`inputB`  

The descriptor of the second input.

`inputBDescriptorType`  

The descriptor type of the second input.

`output`  

The descriptor of the output.

`outputDescriptorType`  

The descriptor type of the output.

`function`  

The arithmetic function.

`activation`  

The activation function that the layer applies to the output.

`filterParameters`  

The filter runtime parameters.

## Discussion

Important

The data types of the inputs must be equal to the output data type. The size of the inputs must either 1, or the maximum size of either input and the output. Arithmetic layers only support arrays with a data type of `float`, and a data layout of BNNS.DataLayout.vector, BNNS.DataLayout.matrixRowMajor, BNNS.DataLayout.matrixColumnMajor, or BNNS.DataLayout.imageCHW.

