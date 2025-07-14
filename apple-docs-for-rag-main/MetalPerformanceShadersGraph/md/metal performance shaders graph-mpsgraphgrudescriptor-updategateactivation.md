

- Metal Performance Shaders Graph
- MPSGraphGRUDescriptor
-  updateGateActivation 

Instance Property

# updateGateActivation

A parameter that defines the activation function to use with the update-gate of the GRU operation.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var updateGateActivation: MPSGraphRNNActivation { get set }
```

## Discussion

Default value: `MPSGraphRNNActivationSigmoid`.

