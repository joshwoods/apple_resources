

- Metal Performance Shaders Graph
- MPSGraphLSTMDescriptor
-  produceCell 

Instance Property

# produceCell

A parameter that controls whether or not to return the output cell from the LSTM layer.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 12.3+tvOS 15.4+visionOS 1.0+

``` source
var produceCell: Bool { get set }
```

## Discussion

If set to `YES` then this layer will produce the internal cell of the LSTM unit as secondary output. Default value: `NO`.

