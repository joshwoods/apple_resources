

- Accelerate
- BNNS
- BNNS.UnaryArithmeticLayer
-  init(input:inputDescriptorType:output:outputDescriptorType:function:activation:filterParameters:) Deprecated

Initializer

# init(input:inputDescriptorType:output:outputDescriptorType:function:activation:filterParameters:)

Returns a new unary arithmetic layer.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
convenience init?(
    input: BNNSNDArrayDescriptor,
    inputDescriptorType: BNNS.DescriptorType,
    output: BNNSNDArrayDescriptor,
    outputDescriptorType: BNNS.DescriptorType,
    function: BNNS.ArithmeticUnaryFunction,
    activation: BNNS.ActivationFunction = .identity,
    filterParameters: BNNSFilterParameters? = nil
)
```

Deprecated

Use the BNNSGraph API instead.

## Parameters 

`input`  

The descriptor of the input.

`inputDescriptorType`  

The descriptor type of the input.

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

The input data type must be equal to the output data type. The input size must equal the output size or `1`. Arithmetic layers only support arrays with a data type of `float`, and a data layout of BNNS.DataLayout.vector, BNNS.DataLayout.matrixRowMajor, BNNS.DataLayout.matrixColumnMajor, or BNNS.DataLayout.imageCHW.

