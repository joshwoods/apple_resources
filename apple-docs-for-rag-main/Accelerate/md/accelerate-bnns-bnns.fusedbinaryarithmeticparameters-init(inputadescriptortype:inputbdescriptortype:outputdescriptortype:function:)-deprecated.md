

- Accelerate
- BNNS
- BNNS.FusedBinaryArithmeticParameters
-  init(inputADescriptorType:inputBDescriptorType:outputDescriptorType:function:) Deprecated

Initializer

# init(inputADescriptorType:inputBDescriptorType:outputDescriptorType:function:)

Returns a new fused binary arithmetic parameters structure.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
init(
    inputADescriptorType: BNNS.DescriptorType,
    inputBDescriptorType: BNNS.DescriptorType,
    outputDescriptorType: BNNS.DescriptorType,
    function: BNNS.ArithmeticBinaryFunction
)
```

Deprecated

Use the BNNSGraph API instead.

## Parameters 

`inputADescriptorType`  

The descriptor type of the first input.

`inputBDescriptorType`  

The descriptor type of the second input.

`outputDescriptorType`  

The descriptor type of the output.

`function`  

The arithmetic function.

