

- Accelerate
- BNNS
- BNNS.TernaryArithmeticLayer
-  init(inputA:inputADescriptorType:inputB:inputBDescriptorType:inputC:inputCDescriptorType:output:outputDescriptorType:function:activation:filterParameters:) Deprecated

Initializer

# init(inputA:inputADescriptorType:inputB:inputBDescriptorType:inputC:inputCDescriptorType:output:outputDescriptorType:function:activation:filterParameters:)

Returns a new ternary arithmetic layer.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+visionOSwatchOS 8.0+tvOS 15.0+

``` source
convenience init?(
    inputA: BNNSNDArrayDescriptor,
    inputADescriptorType: BNNS.DescriptorType,
    inputB: BNNSNDArrayDescriptor,
    inputBDescriptorType: BNNS.DescriptorType,
    inputC: BNNSNDArrayDescriptor,
    inputCDescriptorType: BNNS.DescriptorType,
    output: BNNSNDArrayDescriptor,
    outputDescriptorType: BNNS.DescriptorType,
    function: BNNS.ArithmeticTernaryFunction,
    activation: BNNS.ActivationFunction = .identity,
    filterParameters: BNNSFilterParameters? = nil
)
```

Deprecated

Use the BNNSGraph API instead.

## Parameters 

`inputA`  

The first input descriptor.

`inputADescriptorType`  

The first input descriptor type.

`inputB`  

The second input descriptor.

`inputBDescriptorType`  

The second input descriptor type.

`inputC`  

The first third descriptor.

`inputCDescriptorType`  

The third input descriptor type.

`output`  

The output descriptor.

`outputDescriptorType`  

The output descriptor type.

`function`  

The arithmetic function.

`activation`  

The activation function that the layer applies to the output.

`filterParameters`  

The filter runtime parameters.

