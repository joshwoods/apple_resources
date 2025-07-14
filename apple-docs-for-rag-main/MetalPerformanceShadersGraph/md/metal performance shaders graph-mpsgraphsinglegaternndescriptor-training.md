

- Metal Performance Shaders Graph
- MPSGraphSingleGateRNNDescriptor
-  training 

Instance Property

# training

A parameter that makes the RNN layer support training.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 12.3+tvOS 15.4+visionOS 1.0+

``` source
var training: Bool { get set }
```

## Discussion

If set to `YES` then the layer will produce training state tensor as a secondary output. Default value: `NO`.

