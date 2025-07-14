

- Metal Performance Shaders Graph
- MPSGraphSingleGateRNNDescriptor
-  reverse 

Instance Property

# reverse

A parameter that defines time direction of the input sequence.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 12.3+tvOS 15.4+visionOS 1.0+

``` source
var reverse: Bool { get set }
```

## Discussion

If set to `YES` then the input sequence is passed in reverse time order to the layer. Note: Ignored when `bidirectional = YES`. Default value: `NO`.

