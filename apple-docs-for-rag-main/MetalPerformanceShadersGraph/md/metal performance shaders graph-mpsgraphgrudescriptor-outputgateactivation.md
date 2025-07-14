

- Metal Performance Shaders Graph
- MPSGraphGRUDescriptor
-  outputGateActivation 

Instance Property

# outputGateActivation

A parameter that defines the activation function to use with the output-gate of the GRU operation.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var outputGateActivation: MPSGraphRNNActivation { get set }
```

## Discussion

Default value: `MPSGraphRNNActivationTanh`.

