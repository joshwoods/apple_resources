

- Metal Performance Shaders Graph
- MPSGraphLSTMDescriptor
-  outputGateActivation 

Instance Property

# outputGateActivation

A parameter that defines the activation function used with the output gate of the LSTM operation.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 12.3+tvOS 15.4+visionOS 1.0+

``` source
var outputGateActivation: MPSGraphRNNActivation { get set }
```

## Discussion

Default value: `MPSGraphRNNActivationSigmoid`.

