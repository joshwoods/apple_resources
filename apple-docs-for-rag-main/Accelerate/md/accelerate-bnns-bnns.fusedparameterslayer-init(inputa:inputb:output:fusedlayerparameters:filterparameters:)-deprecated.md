

- Accelerate
- BNNS
- BNNS.FusedParametersLayer
-  init(inputA:inputB:output:fusedLayerParameters:filterParameters:) Deprecated

Initializer

# init(inputA:inputB:output:fusedLayerParameters:filterParameters:)

Creates a new fused layer from an array of layer parameters, where the first layer accepts two inputs.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
convenience init?(
    inputA: BNNSNDArrayDescriptor,
    inputB: BNNSNDArrayDescriptor,
    output: BNNSNDArrayDescriptor,
    fusedLayerParameters: [any FusableLayerParameters],
    filterParameters: BNNSFilterParameters? = nil
)
```

Deprecated

Use the BNNSGraph API instead.

## Parameters 

`inputA`  

The descriptor of the first input.

`inputB`  

The descriptor of the second input.

`output`  

The descriptor of the output.

`fusedLayerParameters`  

An array that contains the parameters of the fused layers.

`filterParameters`  

The runtime filter parameters.

## See Also

### Creating a Fused Parameters Layer

convenience init?(input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, fusedLayerParameters: [any FusableLayerParameters], filterParameters: BNNSFilterParameters?)

Creates a new fused layer from an array of layer parameters.

Deprecated

convenience init?(inputA: BNNSNDArrayDescriptor, inputB: BNNSNDArrayDescriptor, inputC: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, fusedLayerParameters: [any FusableLayerParameters], filterParameters: BNNSFilterParameters?)

Creates a new fused layer from an array of layer parameters, where the first layer accepts three inputs.

Deprecated

