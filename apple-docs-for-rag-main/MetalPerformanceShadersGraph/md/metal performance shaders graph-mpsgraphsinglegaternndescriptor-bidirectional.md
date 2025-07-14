

- Metal Performance Shaders Graph
- MPSGraphSingleGateRNNDescriptor
-  bidirectional 

Instance Property

# bidirectional

A parameter that defines a bidirectional RNN layer.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 12.3+tvOS 15.4+visionOS 1.0+

``` source
var bidirectional: Bool { get set }
```

## Discussion

If set to `YES` then the input sequence is traversed in both directions and the two results are concatenated together on the channel-axis. Default value: `NO`.

