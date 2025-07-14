

- Accelerate
- BNNS
- BNNS.FusedUnaryArithmeticParameters
-  init(inputDescriptorType:outputDescriptorType:function:) Deprecated

Initializer

# init(inputDescriptorType:outputDescriptorType:function:)

Returns a new fused unary arithmetic parameters structure.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+Mac Catalyst

``` source
init(
    inputDescriptorType: BNNS.DescriptorType,
    outputDescriptorType: BNNS.DescriptorType,
    function: BNNS.ArithmeticUnaryFunction
)
```

Deprecated

Use the BNNSGraph API instead.

## Parameters 

`inputDescriptorType`  

The descriptor type of the input.

`outputDescriptorType`  

The descriptor type of the output.

`function`  

The arithmetic function.

